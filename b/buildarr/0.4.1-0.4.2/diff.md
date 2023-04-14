# Comparing `tmp/buildarr-0.4.1.tar.gz` & `tmp/buildarr-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr-0.4.1.tar", max compression
+gzip compressed data, was "buildarr-0.4.2.tar", max compression
```

## Comparing `buildarr-0.4.1.tar` & `buildarr-0.4.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0    35149 2023-04-09 00:59:49.037268 buildarr-0.4.1/LICENSE
--rw-r--r--   0        0        0    14660 2023-04-09 00:59:49.037268 buildarr-0.4.1/README.md
--rw-r--r--   0        0        0      946 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/__init__.py
--rw-r--r--   0        0        0     1783 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/__init__.py
--rw-r--r--   0        0        0    11235 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/compose.py
--rw-r--r--   0        0        0    17974 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/daemon.py
--rw-r--r--   0        0        0     2521 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/exceptions.py
--rw-r--r--   0        0        0     1254 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/main.py
--rw-r--r--   0        0        0    12498 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/run.py
--rw-r--r--   0        0        0     8779 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/test_config.py
--rw-r--r--   0        0        0     1310 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/__init__.py
--rw-r--r--   0        0        0    33589 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/base.py
--rw-r--r--   0        0        0     5429 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/buildarr.py
--rw-r--r--   0        0        0     1071 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/exceptions.py
--rw-r--r--   0        0        0     7213 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/load.py
--rw-r--r--   0        0        0     8853 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/models.py
--rw-r--r--   0        0        0     5338 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/resolve_instance_dependencies.py
--rw-r--r--   0        0        0     2164 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/types.py
--rw-r--r--   0        0        0      827 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/exceptions.py
--rw-r--r--   0        0        0     3046 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/logging.py
--rw-r--r--   0        0        0     6639 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/manager/__init__.py
--rw-r--r--   0        0        0      877 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/manager/exceptions.py
--rw-r--r--   0        0        0      872 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/plugins/dummy/__init__.py
--rw-r--r--   0        0        0     8838 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/plugins/dummy/api.py
--rw-r--r--   0        0        0     2922 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/cli.py
--rw-r--r--   0        0        0     7264 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/config/__init__.py
--rw-r--r--   0        0        0     7783 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/config/settings.py
--rw-r--r--   0        0        0     1184 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/config/types.py
--rw-r--r--   0        0        0     1178 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/exceptions.py
--rw-r--r--   0        0        0      932 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/manager.py
--rw-r--r--   0        0        0     1160 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/plugin.py
--rw-r--r--   0        0        0     3570 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/secrets.py
--rw-r--r--   0        0        0     5934 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/server.py
--rw-r--r--   0        0        0     1386 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/types.py
--rw-r--r--   0        0        0     2236 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/load.py
--rw-r--r--   0        0        0     3728 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/models.py
--rw-r--r--   0        0        0     1239 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/types.py
--rw-r--r--   0        0        0        0 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/py.typed
--rw-r--r--   0        0        0      925 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/secrets/__init__.py
--rw-r--r--   0        0        0     1889 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/secrets/base.py
--rw-r--r--   0        0        0     2466 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/secrets/load.py
--rw-r--r--   0        0        0     3723 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/secrets/models.py
--rw-r--r--   0        0        0     7065 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/state.py
--rw-r--r--   0        0        0     4734 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/trash.py
--rw-r--r--   0        0        0    12955 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/types.py
--rw-r--r--   0        0        0     4183 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/util.py
--rw-r--r--   0        0        0     2326 2023-04-09 00:59:49.041268 buildarr-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    16162 1970-01-01 00:00:00.000000 buildarr-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-14 10:03:59.115044 buildarr-0.4.2/LICENSE
+-rw-r--r--   0        0        0    14660 2023-04-14 10:03:59.115044 buildarr-0.4.2/README.md
+-rw-r--r--   0        0        0      946 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/__init__.py
+-rw-r--r--   0        0        0     1783 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/__init__.py
+-rw-r--r--   0        0        0    11235 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/compose.py
+-rw-r--r--   0        0        0    17974 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/daemon.py
+-rw-r--r--   0        0        0     2521 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/exceptions.py
+-rw-r--r--   0        0        0     1254 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/main.py
+-rw-r--r--   0        0        0    15480 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/run.py
+-rw-r--r--   0        0        0     9627 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/cli/test_config.py
+-rw-r--r--   0        0        0     1402 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/__init__.py
+-rw-r--r--   0        0        0    34135 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/base.py
+-rw-r--r--   0        0        0     5429 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/buildarr.py
+-rw-r--r--   0        0        0     1071 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/exceptions.py
+-rw-r--r--   0        0        0     7213 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/load.py
+-rw-r--r--   0        0        0    10724 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/models.py
+-rw-r--r--   0        0        0     2006 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/render_instance_configs.py
+-rw-r--r--   0        0        0     5338 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/resolve_instance_dependencies.py
+-rw-r--r--   0        0        0     2164 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/config/types.py
+-rw-r--r--   0        0        0      827 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/exceptions.py
+-rw-r--r--   0        0        0     3046 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/logging.py
+-rw-r--r--   0        0        0     9394 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/manager/__init__.py
+-rw-r--r--   0        0        0      877 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/manager/exceptions.py
+-rw-r--r--   0        0        0      872 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/__init__.py
+-rw-r--r--   0        0        0     8838 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/api.py
+-rw-r--r--   0        0        0     2922 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/cli.py
+-rw-r--r--   0        0        0     7264 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/config/__init__.py
+-rw-r--r--   0        0        0     7783 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/config/settings.py
+-rw-r--r--   0        0        0     1184 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/config/types.py
+-rw-r--r--   0        0        0     1178 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/exceptions.py
+-rw-r--r--   0        0        0      932 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/manager.py
+-rw-r--r--   0        0        0     1160 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/plugin.py
+-rw-r--r--   0        0        0     3570 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/secrets.py
+-rw-r--r--   0        0        0     5934 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/server.py
+-rw-r--r--   0        0        0     1386 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/dummy/types.py
+-rw-r--r--   0        0        0     2236 2023-04-14 10:03:59.115044 buildarr-0.4.2/buildarr/plugins/load.py
+-rw-r--r--   0        0        0     3728 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/plugins/models.py
+-rw-r--r--   0        0        0     1239 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/plugins/types.py
+-rw-r--r--   0        0        0        0 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/py.typed
+-rw-r--r--   0        0        0      925 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/secrets/__init__.py
+-rw-r--r--   0        0        0     2807 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/secrets/base.py
+-rw-r--r--   0        0        0     2466 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/secrets/load.py
+-rw-r--r--   0        0        0     3723 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/secrets/models.py
+-rw-r--r--   0        0        0     7334 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/state.py
+-rw-r--r--   0        0        0     5321 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/trash.py
+-rw-r--r--   0        0        0    15383 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/types.py
+-rw-r--r--   0        0        0     4183 2023-04-14 10:03:59.119044 buildarr-0.4.2/buildarr/util.py
+-rw-r--r--   0        0        0     2326 2023-04-14 10:03:59.119044 buildarr-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    16162 1970-01-01 00:00:00.000000 buildarr-0.4.2/PKG-INFO
```

### Comparing `buildarr-0.4.1/LICENSE` & `buildarr-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/README.md` & `buildarr-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/__init__.py` & `buildarr-0.4.2/buildarr/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/cli/__init__.py` & `buildarr-0.4.2/buildarr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/cli/compose.py` & `buildarr-0.4.2/buildarr/cli/compose.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/cli/daemon.py` & `buildarr-0.4.2/buildarr/cli/daemon.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/cli/exceptions.py` & `buildarr-0.4.2/buildarr/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/cli/main.py` & `buildarr-0.4.2/buildarr/cli/main.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/cli/run.py` & `buildarr-0.4.2/buildarr/cli/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,29 +18,39 @@
 
 
 from __future__ import annotations
 
 from logging import getLogger
 from pathlib import Path
 from textwrap import indent
-from typing import Dict, Optional, Set
+from typing import TYPE_CHECKING
 
 import click
 
 from .. import __version__
-from ..config import load_config, load_instance_configs, resolve_instance_dependencies
+from ..config import (
+    load_config,
+    load_instance_configs,
+    render_instance_configs,
+    resolve_instance_dependencies,
+)
 from ..logging import get_log_level
 from ..manager import load_managers
-from ..secrets import SecretsPlugin, load_secrets
+from ..secrets import load_secrets
 from ..state import state
 from ..trash import fetch_trash_metadata, render_trash_metadata, trash_metadata_used
-from ..util import create_temp_dir, get_resolved_path
+from ..util import get_resolved_path
 from . import cli
 from .exceptions import RunInstanceConnectionTestFailedError, RunNoPluginsDefinedError
 
+if TYPE_CHECKING:
+    from typing import Dict, Optional, Set
+
+    from ..secrets import SecretsPlugin
+
 logger = getLogger(__name__)
 
 
 @cli.command(
     help=(
         "Update configured instances, and exit.\n\n"
         "If CONFIG-PATH is not defined, use `buildarr.yml' from the current directory."
@@ -186,14 +196,61 @@
     logger.info("Resolving instance dependencies")
     resolve_instance_dependencies()
     logger.debug("Execution order:")
     for i, (plugin_name, instance_name) in enumerate(state._execution_order, 1):
         logger.debug("  %i. %s.instances[%s]", i, plugin_name, repr(instance_name))
     logger.info("Finished resolving instance dependencies")
 
+    # Render dynamically populated attributes in instance configurations,
+    # with the TRaSH-Guides metadata directory available in the global state
+    # only if at least one instance configuration requires it.
+    if trash_metadata_used():
+        logger.info("Fetching TRaSH metadata")
+        with fetch_trash_metadata() as trash_metadata_dir:
+            # TODO: Remove `render_trash_metadata` in Buildarr v0.5.0.
+            logger.info("Finished fetching TRaSH metadata")
+            logger.info("Rendering TRaSH metadata")
+            render_trash_metadata(trash_metadata_dir)
+            logger.info("Finished rendering TRaSH metadata")
+            logger.info("Rendering instance configuration dynamic attributes")
+            render_instance_configs()
+            logger.info("Finished rendering instance configuration dynamic attributes")
+    else:
+        logger.info("Rendering instance configuration dynamic attributes")
+        render_instance_configs()
+        logger.info("Finished rendering instance configuration dynamic attributes")
+
+    # Initialise any instances that have not been initialised yet.
+    # For applicable instances, this needs to be done before the main API can be queried,
+    # or secrets can even be checked.
+    for plugin_name, instance_name in state._execution_order:
+        manager = state.managers[plugin_name]
+        instance_config = state.instance_configs[plugin_name][instance_name]
+        with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
+            logger.debug("Checking if the instance is initialised")
+            try:
+                is_initialized = manager.is_initialized(instance_config)
+            except NotImplementedError:
+                logger.debug("Initialisation is not required for this instance type")
+                continue
+            if is_initialized:
+                logger.debug("Instance is initialised and ready for configuration updates")
+            else:
+                logger.info("Instance has not been initialised")
+                logger.info("Initialising instance")
+                manager.initialize(
+                    (
+                        plugin_name
+                        if instance_name == "default"
+                        else f"{plugin_name}.instances[{repr(instance_config)}]"
+                    ),
+                    instance_config,
+                )
+                logger.info("Finished initialising instance")
+
     # Load the secrets file if it exists, and initialise the secrets metadata.
     # If `use_plugins` is undefined, load using all plugins available
     # to preserve cached secrets metadata that isn't used.
     logger.info("Loading secrets file from '%s'", secrets_file_path)
     if load_secrets(path=secrets_file_path, use_plugins=use_plugins):
         logger.info("Finished loading secrets file")
     else:
@@ -233,77 +290,77 @@
                 logger.info("Finished checking secrets")
 
     # Save the latest secrets file to disk.
     logger.info("Saving updated secrets file to '%s'", secrets_file_path)
     state.secrets.write(secrets_file_path)
     logger.info("Finished saving updated secrets file")
 
-    # Render any instance configuration with TRaSH-Guides metadata referenced,
-    # populating any missing values.
-    if trash_metadata_used():
-        logger.debug("Creating TRaSH metadata directory")
-        with create_temp_dir() as trash_metadata_dir:
-            logger.debug("Finished creating TRaSH metadata directory")
-            logger.info("Fetching TRaSH metadata")
-            fetch_trash_metadata(trash_metadata_dir)
-            logger.info("Finished fetching TRaSH metadata")
-            logger.info("Rendering TRaSH metadata")
-            render_trash_metadata(trash_metadata_dir)
-            logger.info("Finished rendering TRaSH metadata")
-
     # Update all instances in the determined execution order.
     logger.info("Updating configuration on remote instances")
-
     for plugin_name, instance_name in state._execution_order:
         manager = state.managers[plugin_name]
         instance_config = state.instance_configs[plugin_name][instance_name]
         with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
-            # Get the instance's secrets metadata.
             instance_secrets = getattr(state.secrets, plugin_name)[instance_name]
-
-            # Fetch the current active configuration from the remote instance,
-            # so it can be compared to the local configuration.
-            logger.info("Getting remote configuration")
+            logger.info("Fetching remote configuration to check if updates are required")
             remote_instance_config = manager.from_remote(instance_config, instance_secrets)
-            logger.info("Finished getting remote configuration")
-
-            # Output the local and remote instance configuration to the debug logs,
-            # so they can be inspected to see Buildarr's state at this point, if need be.
+            logger.info("Finished fetching remote configuration")
             for config_type, config in (
                 ("Local", instance_config),
                 ("Remote", remote_instance_config),
             ):
                 logger.debug("%s configuration:", config_type)
                 for config_line in config.yaml(exclude_unset=True).splitlines():
                     logger.debug(indent(config_line, "  "))
-
-            # Compare the local configuration for the instance to the active configuration,
-            # and if there are differences, update the instance.
             logger.info("Updating remote configuration")
             logger.info(
                 (
                     "Remote configuration successfully updated"
                     if manager.update_remote(
                         plugin_name,
                         instance_config,
                         instance_secrets,
                         remote_instance_config,
                     )
                     else "Remote configuration is up to date"
                 ),
             )
             logger.info("Finished updating remote configuration")
-
-            # TODO: Re-fetch the remote configuration and test that it
-            #       now matches the local configuration.
-            # print("Re-fetching remote config")
-            # new_active_config = manager.get_active_config(
-            #     instance_config,
-            #     getattr(secrets, manager_name),
-            # )
-            # print(
-            #     "Active configuration for instance name "
-            #     f'{instance_name}' after update:\n"
-            #     f"{pformat(new_active_config.dict(exclude_unset=True))}",
-            # )
-
     logger.info("Finished updating configuration on remote instances")
+
+    # After all configuration and resources have been created/updated on
+    # the remote instances, make another pass and remove any unmanaged or
+    # unused resources slated for deletion.
+    # The execution order is the reverse of the normal order, to ensure
+    # any resources on source instances that depend on resources on
+    # target instances (via instance links) are removed first.
+    logger.info("Deleting unmanaged/unused resources on remote instances")
+    for plugin_name, instance_name in reversed(state._execution_order):
+        manager = state.managers[plugin_name]
+        instance_config = state.instance_configs[plugin_name][instance_name]
+        with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
+            instance_secrets = getattr(state.secrets, plugin_name)[instance_name]
+            logger.info("Refetching remote configuration to delete unused resources")
+            remote_instance_config = manager.from_remote(instance_config, instance_secrets)
+            logger.info("Finished refetching remote configuration")
+            for config_type, config in (
+                ("Local", instance_config),
+                ("Remote", remote_instance_config),
+            ):
+                logger.debug("%s configuration:", config_type)
+                for config_line in config.yaml(exclude_unset=True).splitlines():
+                    logger.debug(indent(config_line, "  "))
+            logger.info("Deleting unmanaged/unused resources on the remote instance")
+            logger.info(
+                (
+                    "Unused resources successfully deleted"
+                    if manager.delete_remote(
+                        plugin_name,
+                        instance_config,
+                        instance_secrets,
+                        remote_instance_config,
+                    )
+                    else "Remote configuration is clean"
+                ),
+            )
+            logger.info("Finished deleting unmanaged/unused resources on the remote instance")
+    logger.info("Finished deleting unmanaged/unused resources on remote instances")
```

### Comparing `buildarr-0.4.1/buildarr/cli/test_config.py` & `buildarr-0.4.2/buildarr/cli/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,25 @@
 from pathlib import Path
 from textwrap import indent
 from typing import TYPE_CHECKING
 
 import click
 
 from .. import __version__
-from ..config import load_config, load_instance_configs, resolve_instance_dependencies
+from ..config import (
+    load_config,
+    load_instance_configs,
+    render_instance_configs,
+    resolve_instance_dependencies,
+)
 from ..logging import get_log_level
 from ..manager import load_managers
 from ..state import state
 from ..trash import fetch_trash_metadata, render_trash_metadata
-from ..util import create_temp_dir, get_resolved_path
+from ..util import get_resolved_path
 from . import cli
 from .exceptions import TestConfigNoPluginsDefinedError
 
 if TYPE_CHECKING:
     from typing import Set
 
 
@@ -163,52 +168,67 @@
         for instance_config in state.instance_configs[plugin_name].values():
             if state.managers[plugin_name].uses_trash_metadata(instance_config):
                 uses_trash_metadata = True
                 break
         if uses_trash_metadata:
             break
 
-    # Skip this test if no configuration uses TRaSH-Guides metadata,
-    # but otherwise, create a temporary directory, download the TRaSH-Guides metadata,
-    # and render the metadata into the instance-specific configurations.
-    if not uses_trash_metadata:
-        logger.info("Fetching TRaSH-Guides metadata: SKIPPED (not required)")
-        logger.info("Rendering TRaSH-Guides metadata: SKIPPED (not required)")
-    else:
-        logger.debug("Creating TRaSH metadata directory")
-        with create_temp_dir() as trash_metadata_dir:
-            logger.debug("Finished creating TRaSH metadata directory")
-            try:
-                logger.debug("Fetching TRaSH metadata")
-                fetch_trash_metadata(trash_metadata_dir)
+    # Test rendering the instance configuration.
+    # If the TRaSH-Guides metadata is required by the configuration, run the rendering
+    # with the TRaSH-Guides metadata available.
+    # If the configuration reports that TRaSH-Guides metadata is not required,
+    # run the test without fetching it.
+    if uses_trash_metadata:
+        fetching_metadata = True
+        try:
+            logger.debug("Fetching TRaSH metadata")
+            with fetch_trash_metadata() as trash_metadata_dir:
                 logger.debug("Finished fetching TRaSH metadata")
-            except Exception:
-                logger.error("Fetching TRaSH-Guides metadata: FAILED")
-                raise
-            else:
                 logger.info("Fetching TRaSH-Guides metadata: PASSED")
-            try:
-                logger.debug("Rendering TRaSH metadata")
-                render_trash_metadata(trash_metadata_dir)
-                logger.debug("Finished rendering TRaSH metadata")
-            except Exception:
-                logger.error("Rendering TRaSH-Guides metadata: FAILED")
-                raise
-            else:
-                for plugin_name, instance_configs in state.instance_configs.items():
-                    for instance_name, instance_config in instance_configs.items():
-                        with state._with_context(
-                            plugin_name=plugin_name,
-                            instance_name=instance_name,
-                        ):
-                            if state.managers[plugin_name].uses_trash_metadata(instance_config):
-                                logger.debug("Rendered instance configuration:")
-                                for config_line in instance_config.yaml(
-                                    exclude_unset=True,
-                                ).splitlines():
-                                    logger.debug(indent(config_line, "  "))
-                logger.info("Rendering TRaSH-Guides metadata: PASSED")
+                fetching_metadata = False
+                # TODO: Remove `render_trash_metadata` in Buildarr v0.5.0.
+                try:
+                    logger.debug("Rendering TRaSH metadata")
+                    render_trash_metadata(trash_metadata_dir)
+                    logger.debug("Finished rendering TRaSH metadata")
+                except Exception:
+                    logger.error("Rendering TRaSH-Guides metadata: FAILED")
+                    raise
+                else:
+                    logger.info("Rendering TRaSH-Guides metadata: PASSED")
+                try:
+                    logger.debug("Rendering instance configuration dynamic attributes")
+                    render_instance_configs()
+                    logger.debug("Finished rendering instance configuration dynamic attributes")
+                except Exception:
+                    logger.error("Rendering instance configuration dynamic attributes: FAILED")
+                    raise
+                else:
+                    logger.info("Rendering instance configuration dynamic attributes: PASSED")
+        except Exception:
+            if fetching_metadata:
+                logger.error("Fetching TRaSH-Guides metadata: FAILED")
+            raise
+    else:
+        logger.info("Fetching TRaSH-Guides metadata: SKIPPED (not required)")
+        logger.info("Rendering TRaSH-Guides metadata: SKIPPED (not required)")
+        try:
+            logger.debug("Rendering instance configuration dynamic attributes")
+            render_instance_configs()
+            logger.debug("Finished rendering instance configuration dynamic attributes")
+        except Exception:
+            logger.error("Rendering instance configuration dynamic attributes: FAILED")
+            raise
+        else:
+            logger.info("Rendering instance configuration dynamic attributes: PASSED")
+    for plugin_name, instance_configs in state.instance_configs.items():
+        for instance_name, instance_config in instance_configs.items():
+            with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
+                if state.managers[plugin_name].uses_trash_metadata(instance_config):
+                    logger.debug("Rendered instance configuration:")
+                    for config_line in instance_config.yaml(exclude_unset=True).splitlines():
+                        logger.debug(indent(config_line, "  "))
 
     # If we get to this point, this configuration is pretty much guaranteed to be valid.
     # Incorrect values for a remote application instance notwithstanding, it should
     # work properly in a real Buildarr run.
     logger.info("Configuration test successful.")
```

### Comparing `buildarr-0.4.1/buildarr/config/__init__.py` & `buildarr-0.4.2/buildarr/config/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 
 from __future__ import annotations
 
 from .base import ConfigBase
 from .exceptions import ConfigError, ConfigTrashIDNotFoundError
 from .load import load_config, load_instance_configs
 from .models import ConfigPlugin, ConfigPluginType, ConfigType
+from .render_instance_configs import render_instance_configs
 from .resolve_instance_dependencies import resolve_instance_dependencies
 from .types import RemoteMapEntry
 
 __all__ = [
     "ConfigError",
     "ConfigTrashIDNotFoundError",
     "ConfigBase",
     "ConfigPlugin",
     "ConfigType",
     "ConfigPluginType",
     "RemoteMapEntry",
     "load_config",
     "load_instance_configs",
     "resolve_instance_dependencies",
+    "render_instance_configs",
 ]
```

### Comparing `buildarr-0.4.1/buildarr/config/base.py` & `buildarr-0.4.2/buildarr/config/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from pathlib import Path, PurePosixPath
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
+    List,
     Mapping,
     Optional,
     Set,
     Tuple,
     Type,
     Union,
     get_args as get_type_args,
@@ -43,15 +44,15 @@
 import yaml
 
 from pydantic import AnyUrl, BaseModel, SecretStr
 from pydantic.validators import _VALIDATORS
 from typing_extensions import Self
 
 from ..plugins import Secrets
-from ..types import BaseEnum, BaseIntEnum
+from ..types import BaseEnum, BaseIntEnum, ModelConfigBase
 from .types import RemoteMapEntry
 
 logger = getLogger(__name__)
 
 OPTIONAL_TYPE_UNION_SIZE = 2
 
 
@@ -630,26 +631,61 @@
                         {"name": remote_attr_name, "value": encoded_value},
                     )
                 else:
                     remote_attrs[remote_attr_name] = encoded_value
         # Return the completed remote attribute dictionary structure.
         return (changed, remote_attrs)
 
+    def delete_remote(
+        self,
+        tree: str,
+        secrets: Secrets,
+        remote: Self,
+    ) -> bool:
+        """
+        Compare the local configuration to a remote instance, and delete any resources
+        that are unmanaged or unused on the remote, and allowed to be deleted.
+
+        This function should be overloaded by implementing classes with resources that
+        may need to be deleted from a remote instance if it is unmanaged by Buildarr
+        or simply unused.
+
+        The base function simply implements traversing the configuration tree
+        to call child section functions.
+
+        Args:
+            tree (str): Configuration tree represented as a string. Mainly used in logging.
+            secrets (Secrets): Remote instance host and secrets information.
+            remote (Self): Remote instance configuration for the current section.
+
+        Returns:
+            `True` if the remote configuration changed, otherwise `False`
+        """
+        changed = False
+        for field_name, field in self:
+            if isinstance(field, ConfigBase) and field.delete_remote(
+                f"{tree}.{field_name}",
+                secrets,
+                getattr(remote, field_name),
+            ):
+                changed = True
+        return changed
+
     @classmethod
     def _format_attr(cls, value: Any) -> Any:
         """
         Default configuration value formatting function.
 
         Args:
             value (Any): Value to format
 
         Returns:
             The value to pass to the logging function
         """
-        if isinstance(value, BaseEnum):
+        if isinstance(value, (BaseEnum, BaseIntEnum)):
             return value.to_name_str()
         elif isinstance(value, AnyUrl):
             return str(value)
         elif isinstance(value, SecretStr):
             return str(value)
         elif isinstance(value, Path):
             return str(value)
@@ -669,50 +705,55 @@
         Args:
             attr_name (str): Name of attribute to decode
             value (Any): Remote attribute value
 
         Returns:
             Local attribute value
         """
-        return cls._decode_attr_(cls.__fields__[attr_name].type_, value)
+        return cls._decode_attr_(cls.__fields__[attr_name].outer_type_, value)
 
     @classmethod
     def _decode_attr_(cls, attr_type: Type[Any], value: Any) -> Any:
-        if get_type_origin(attr_type) is list:
-            return [cls._decode_attr_(get_type_args(attr_type)[0], v) for v in value]
-        elif get_type_origin(attr_type) is set:
-            return set(cls._decode_attr_(get_type_args(attr_type)[0], v) for v in value)
-        elif get_type_origin(attr_type) is Union:
-            attr_union_types = get_type_args(attr_type)
+        type_tree: List[Type[Any]] = [attr_type]
+        while get_type_origin(type_tree[-1]) is not None:
+            origin_type = get_type_origin(type_tree[-1])
+            if origin_type is not None:
+                type_tree.append(origin_type)
+        if type_tree[-1] is list:
+            return [cls._decode_attr_(get_type_args(type_tree[-2])[0], v) for v in value]
+        elif type_tree[-1] is set:
+            return set(cls._decode_attr_(get_type_args(type_tree[-2])[0], v) for v in value)
+        elif type_tree[-1] is Union:
+            attr_union_types = get_type_args(type_tree[-2])
             #
             if (
                 len(attr_union_types) == OPTIONAL_TYPE_UNION_SIZE
                 and type(None) in attr_union_types
                 and value is not None
             ):
                 return cls._decode_attr(
                     [t for t in attr_union_types if t is not type(None)][0],
                     value,
                 )
-        elif issubclass(attr_type, BaseEnum):
-            return attr_type(value)
+        elif issubclass(type_tree[-1], (BaseEnum, BaseIntEnum)):
+            return type_tree[-1](value)
         return value
 
     @classmethod
     def _encode_attr(cls, value: Any) -> Any:
         """
         Default local-to-remote instance attribute encoding function.
 
         Args:
             value (Any): Local attribute value
 
         Returns:
             Remote attribute value
         """
-        if isinstance(value, BaseEnum):
+        if isinstance(value, (BaseEnum, BaseIntEnum)):
             return value.value
         elif isinstance(value, AnyUrl):
             return str(value)
         elif isinstance(value, SecretStr):
             return value.get_secret_value()
         elif isinstance(value, UUID):
             return str(value)
@@ -741,68 +782,46 @@
             YAML representation of the model
         """
         return yaml.safe_dump(  # type: ignore[call-overload]
             json.loads(self.json(*args, **kwargs)),
             **{**(yaml_kwargs or {}), "sort_keys": sort_keys},
         )
 
-    class Config:
+    class Config(ModelConfigBase):
         """
-        Buildarr base Pydantic model configuration.
+        Buildarr configuration model class settings.
 
-        Sets some required configuration parameters for
-        serialisation and parsing to work correctly.
+        Sets some required parameters for serialisation,
+        parsing and validation to work correctly.
 
         To set additional parameters in your implementing class, subclass this class:
 
         ```python
         from __future__ import annotations
 
         from typing import TYPE_CHECKING
         from buildarr.config import ConfigBase
 
         if TYPE_CHECKING:
             from .secrets import ExampleSecrets
-            class ExampleConfigBase(ConfigBase[ExampleSecrets]):
+            class _ExampleConfig(ConfigBase[ExampleSecrets]):
                 ...
         else:
-            class ExampleConfigBase(ConfigBase):
+            class _ExampleConfig(ConfigBase):
                 ...
 
-        class ExampleConfig(ExampleConfigBase):
+        class ExampleConfig(_ExampleConfig):
             ...
 
-            class Config(ExampleConfigBase.Config):
+            class Config(_ExampleConfig.Config):
                 ...  # Add model configuration attributes here.
         ```
         """
 
-        # Add default JSON encoders for custom, non-default and otherwise non-specified
-        # classes so serialisation can work.
-        json_encoders = {
-            BaseEnum: lambda v: v.to_name_str(),
-            BaseIntEnum: lambda v: v.to_name_str(),
-            PurePosixPath: str,
-            SecretStr: lambda v: v.get_secret_value(),
-        }
-
-        # Required to avoid coersion with same-name but different-typed fields
-        # in objects for which there are multiple types that can be defined.
-        smart_union = True
-
-        # When aliases are defined, allow attributes to be referenced by their
-        # internal name, as well as the alias.
-        allow_population_by_field_name = True
-
-        # Validate all configuration attributes, even the default ones.
-        # This is necessary because the default attributes sometimes need to
-        # be validated for correctness in non-default contexts.
-        # (For example, a normally optional attribute becoming required due to
-        # another attribute being enabled.)
-        validate_all = True
+        pass
 
 
 def _validate_pure_posix_path(v: Any) -> PurePosixPath:
     """
     PurePosixPath default object validator for Pydantic.
 
     Args:
```

### Comparing `buildarr-0.4.1/buildarr/config/buildarr.py` & `buildarr-0.4.2/buildarr/config/buildarr.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/config/exceptions.py` & `buildarr-0.4.2/buildarr/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/config/load.py` & `buildarr-0.4.2/buildarr/config/load.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/config/models.py` & `buildarr-0.4.2/buildarr/config/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -194,14 +194,60 @@
             trash_metadata_dir (Path): TRaSH-Guides metadata directory.
 
         Returns:
             Rendered configuration object
         """
         return self
 
+    def render(self) -> Self:
+        """
+        Render any dynamically populated attributes in this instance configuration.
+
+        Configuration plugins should implement this function if there are any attributes
+        that get dynamically populated, e.g. TRaSH-Guides metadata.
+
+        Returns:
+            Rendered configuration object
+        """
+        return self
+
+    def is_initialized(self) -> bool:
+        """
+        Return whether or not this instance needs to be initialised.
+
+        This function runs after the instance configuration has been rendered,
+        but before secrets are fetched.
+
+        Configuration plugins should implement this function if initialisation is required
+        for the application's API to become available.
+
+        Raises:
+            NotImplementedError: When initialisation is not required for the application type.
+
+        Returns:
+            `True` if the instance is initialised, otherwise `False`
+        """
+        raise NotImplementedError()
+
+    def initialize(self, tree: str) -> None:
+        """
+        Initialise the instance, and make the main application API available for Buildarr
+        to query against.
+
+        This function runs after the instance configuration has been rendered,
+        but before secrets are fetched.
+
+        Configuration plugins should implement this function if initialisation is required
+        for the application's API to become available.
+
+        Args:
+            tree (str): Configuration tree this instance falls under (for logging purposes).
+        """
+        raise NotImplementedError()
+
     def to_compose_service(self, compose_version: str, service_name: str) -> Dict[str, Any]:
         """
         Generate a Docker Compose service definition corresponding to this instance configuration.
 
         Plugins should implement this function to allow Docker Compose files to be generated from
         Buildarr configuration using the `buildarr compose` command.
 
@@ -228,14 +274,19 @@
             Dict[str, Any]: Changed field structure
         """
         if "instances" in values:
             for instance_name, instance in cast(
                 Dict[str, ConfigPlugin],
                 values["instances"],
             ).items():
+                if instance_name == "default":
+                    raise ValueError(
+                        "instance name 'default' is reserved within Buildarr, "
+                        "please choose a different name for this instance",
+                    )
                 if "hostname" not in instance.__fields_set__:
                     instance.hostname = instance_name  # type: ignore[assignment]
         return values
 
 
 class ConfigPluginType(ConfigPlugin):
     """
```

### Comparing `buildarr-0.4.1/buildarr/config/resolve_instance_dependencies.py` & `buildarr-0.4.2/buildarr/config/resolve_instance_dependencies.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/config/types.py` & `buildarr-0.4.2/buildarr/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/exceptions.py` & `buildarr-0.4.2/buildarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/logging.py` & `buildarr-0.4.2/buildarr/logging.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/manager/__init__.py` & `buildarr-0.4.2/buildarr/plugins/dummy/config/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,179 +9,236 @@
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Buildarr.
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
-Buildarr manager interface.
+Dummy plugin configuration.
 """
 
 
 from __future__ import annotations
 
-from logging import getLogger
-from typing import TYPE_CHECKING, Generic
+from pathlib import Path
+from typing import TYPE_CHECKING, Dict, Optional
 
-from ..plugins import Config, Secrets
-from ..state import state
+from typing_extensions import Self
 
+from buildarr.config import ConfigPlugin
+from buildarr.types import NonEmptyStr, Port
+
+from ..api import api_get
+from ..secrets import DummySecrets
+from ..types import DummyApiKey, DummyProtocol
+from .settings import DummySettingsConfig
+
+# Allow Mypy to properly resolve secrets type declarations in configuration classes.
 if TYPE_CHECKING:
-    from pathlib import Path
-    from typing import Any, Dict, Optional, Set
 
+    class _DummyInstanceConfig(ConfigPlugin[DummySecrets]):
+        ...
 
-logger = getLogger(__name__)
+else:
 
+    class _DummyInstanceConfig(ConfigPlugin):
+        ...
 
-class ManagerPlugin(Generic[Config, Secrets]):
+
+class DummyInstanceConfig(_DummyInstanceConfig):
     """
-    Buildarr plugin manager object base class.
+    By default, Buildarr will look for a single instance at `http://dummy:5000`.
+    Most configurations are different, and to accommodate those, you can configure
+    how Buildarr connects to individual Dummy instances.
+
+    Configuration of a single Dummy instance:
+
+    ```yaml
+    dummy:
+      hostname: "localhost"
+      port: 5000
+      protocol: "http"
+      settings:
+        ...
+    ```
 
-    This class contains functions used by the Buildarr main routine to
-    interact with a plugin's configuration and secrets interfaces.
+    Configuration of multiple instances:
+
+    ```yaml
+    dummy:
+      # Configuration and settings common to all instances.
+      hostname: "localhost"
+      protocol: "http"
+      settings:
+        ...
+      instances:
+        # Dummy instance 1-specific configuration.
+        dummy1:
+          port: 5000
+          settings:
+            ...
+        # Dummy instance 2-specific configuration.
+        dummy:
+          port: 5001
+          api_key: "..." # Explicitly define API key
+          settings:
+            ...
+    ```
+    """
 
-    In most cases these do not need to be modified and plugins can
-    subclass the default `ManagerPlugin` interface without any issues, but all
-    hooks can be overloaded and reimplemented if desired.
+    hostname: NonEmptyStr = "dummy"  # type: ignore[assignment]
+    """
+    Hostname of the Dummy instance to connect to.
 
-    `ManagerPlugin` is a generic interface, so to create the manager class
-    for your plugin, create a class with `ManagerPlugin` as the superclass,
-    with the configuration and secrets classes for your plugin passed into
-    the appropriate type parameters.
+    When defining a single instance using the global `dummy` configuration block,
+    the default hostname is `dummy`.
 
-    ```python
-    from buildarr.manager import ManagerPlugin
-    from .config import ExampleConfig
-    from .secrets import ExampleSecrets
+    When using multiple instance-specific configurations, the default hostname
+    is the name given to the instance in the `instances` attribute.
 
-    class ExampleManager(ManagerPlugin[ExampleConfig, ExampleSecrets]):
-        pass
+    ```yaml
+    dummy:
+      instances:
+        dummy1: # <--- This becomes the default hostname
+          ...
     ```
+    """
 
-    If your plugin has distinct classes for global configuration and
-    instance-specific configuration (e.g. `ExampleConfig` and `ExampleInstanceConfig`),
-    pass `ExampleInstanceConfig` to `ExampleManager`.
+    port: Port = 5000  # type: ignore[assignment]
+    """
+    Port number of the Dummy instance to connect to.
     """
 
-    def get_instance_config(self, config: Config, instance_name: str) -> Config:
-        """
-        Combine explicitly defined instance-local and global configuration,
-        and return a fully qualified instance-specific plugin configuration object.
+    protocol: DummyProtocol = "http"  # type: ignore[assignment]
+    """
+    Communication protocol to use to connect to Dummy.
 
-        Args:
-            config (Config): Configuration object to read.
-            instance_name (str): Name of the instance to get the configuration of.
+    Values:
 
-        Returns:
-            Fully qualified instance-specific configuration object
-        """
-        return config.get_instance_config(instance_name)
+    * `http`
+    """
 
-    def uses_trash_metadata(self, instance_config: Config) -> bool:
-        """
-        Returns whether or not the given instance configuration uses TRaSH-Guides metadata.
+    api_key: Optional[DummyApiKey] = None
+    """
+    API key to use to authenticate with the Dummy instance.
 
-        Args:
-            instance_config (Config): Instance configuration object to check.
+    If undefined or set to `None`, automatically retrieve the API key.
+    This can only be done on Dummy instances with authentication disabled.
+    """
+
+    version: Optional[str] = None
+    """
+    The expected version of the Dummy instance.
+    If undefined or set to `None`, the version is auto-detected.
+
+    At the moment this attribute is unused, and there is likely no need to explicitly set it.
+    """
+
+    settings: DummySettingsConfig = DummySettingsConfig()
+    """
+    Dummy settings.
+    Configuration options for Dummy itself are set within this structure.
+    """
+
+    @property
+    def uses_trash_metadata(self) -> bool:
+        """
+        A flag determining whether or not this instance configuration uses TRaSH-Guides metadata.
 
         Returns:
             `True` if TRaSH-Guides metadata is used, otherwise `False`
         """
-        return instance_config.uses_trash_metadata
+        return self.settings.uses_trash_metadata
 
-    def render_trash_metadata(self, instance_config: Config, trash_metadata_dir: Path) -> Config:
+    def render_trash_metadata(self, trash_metadata_dir: Path) -> Self:
         """
-        Read TRaSH-Guides metadata, and return an instance configuration object
-        with all templates rendered.
+        Read TRaSH-Guides metadata, and return a configuration object with all templates rendered.
 
         Args:
-            instance_config (Config): Instance configuration object to render.
             trash_metadata_dir (Path): TRaSH-Guides metadata directory.
 
         Returns:
             Rendered configuration object
         """
-        return instance_config.render_trash_metadata(trash_metadata_dir)
+        copy = self.copy(deep=True)
+        copy._render_trash_metadata(trash_metadata_dir)
+        return copy
 
-    def from_remote(self, instance_config: Config, secrets: Secrets) -> Config:
+    def _render_trash_metadata(self, trash_metadata_dir: Path) -> None:
         """
-        Get the active configuration for a remote instance, and return the resulting object.
+        Render configuration attributes obtained from TRaSH-Guides, in-place.
 
         Args:
-            instance_config (Config): Configuration object of the instance to connect to.
-            secrets (Secrets): Remote instance host and secrets information.
-
-        Returns:
-            Remote instance configuration object
+            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
         """
-        return instance_config.from_remote(secrets)
+        if self.settings.uses_trash_metadata:
+            self.settings._render_trash_metadata(trash_metadata_dir)
 
-    def update_remote(
-        self,
-        tree: str,
-        local_instance_config: Config,
-        secrets: Secrets,
-        remote_instance_config: Config,
-    ) -> bool:
+    @classmethod
+    def from_remote(cls, secrets: DummySecrets) -> Self:
         """
-        Compare the local configuration to a remote instance, and update the remote to match.
+        Read configuration from a remote instance and return it as a configuration object.
 
         Args:
-            tree (str): Configuration tree represented as a string. Mainly used in logging.
-            local_instance_config (Config): Local instance configuration to compare to the remote.
-            secrets (Secrets): Remote instance host and secrets information.
-            remote_instance_config (Config): Currently active remote instance configuration.
+            secrets (DummySecrets): Instance host and secrets information
 
         Returns:
-            `True` if the remote configuration changed, otherwise `False`
+            Configuration object for remote instance
         """
-        return local_instance_config.update_remote(
-            tree=tree,
-            secrets=secrets,
-            remote=remote_instance_config,
+        return cls(
+            hostname=secrets.hostname,
+            port=secrets.port,
+            protocol=secrets.protocol,
+            api_key=secrets.api_key,
+            version=api_get(secrets, "/api/v1/status")["version"],
+            settings=DummySettingsConfig.from_remote(secrets),
         )
 
-    def to_compose_service(
-        self,
-        instance_config: Config,
-        compose_version: str,
-        service_name: str,
-    ) -> Dict[str, Any]:
-        """
-        Generate a Docker Compose service definition corresponding to this instance configuration.
 
-        Args:
-            instance_config (Config): Instance configuration to generate a service for.
-            compose_version (str): Version of the Docker Compose file.
-            service_name (str): The unique name for the generated Docker Compose service.
-
-        Returns:
-            Docker Compose service definition dictionary
-        """
-        return instance_config.to_compose_service(
-            compose_version=compose_version,
-            service_name=service_name,
-        )
+class DummyConfig(DummyInstanceConfig):
+    """
+    Dummy plugin global configuration class.
 
+    Subclasses the instance-specific configuration to allow
+    attributes common to all instances to be defined in one place.
+    """
 
-def load_managers(use_plugins: Optional[Set[str]] = None) -> None:
+    instances: Dict[str, DummyInstanceConfig] = {}
     """
-    Load the managers for each plugin to be used in this Buildarr run.
+    Instance-specific Dummy configuration.
 
-    Args:
-        use_plugins (Optional[Set[str]]): Plugins to use. Default is to use all plugins.
+    Can only be defined on the global `dummy` configuration block.
+
+    Globally specified configuration values apply to all instances.
+    Configuration values specified on an instance-level take precedence at runtime.
     """
 
-    managers: Dict[str, ManagerPlugin] = {}
+    @property
+    def uses_trash_metadata(self) -> bool:
+        """
+        A flag determining whether or not this configuration uses TRaSH-Guides metadata.
 
-    for plugin_name, plugin in state.plugins.items():
-        if use_plugins and plugin_name not in use_plugins:
-            continue
-        if plugin_name not in state.config.__fields_set__:
-            continue
-        with state._with_context(plugin_name=plugin_name):
-            logger.debug("Loading plugin manager")
-            managers[plugin_name] = plugin.manager()
-            logger.debug("Finished loading plugin manager")
+        Returns:
+            `True` if TRaSH-Guides metadata is used, otherwise `False`
+        """
+        for instance in self.instances.values():
+            if instance.uses_trash_metadata:
+                return True
+        return super().uses_trash_metadata
+
+    def render_trash_metadata(self, trash_metadata_dir: Path) -> Self:
+        """
+        Read TRaSH-Guides metadata, and return a configuration object with all templates rendered.
 
-    state.managers = managers
+        Args:
+            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
+
+        Returns:
+            Rendered configuration object
+        """
+        copy = self.copy(deep=True)
+        for instance in copy.instances.values():
+            if instance.uses_trash_metadata:
+                instance._render_trash_metadata(trash_metadata_dir)
+        if self.uses_trash_metadata:
+            copy._render_trash_metadata(trash_metadata_dir)
+        return copy
```

### Comparing `buildarr-0.4.1/buildarr/manager/exceptions.py` & `buildarr-0.4.2/buildarr/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/__init__.py` & `buildarr-0.4.2/buildarr/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/api.py` & `buildarr-0.4.2/buildarr/plugins/dummy/api.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/cli.py` & `buildarr-0.4.2/buildarr/plugins/dummy/cli.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/config/__init__.py` & `buildarr-0.4.2/buildarr/state.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,236 +9,224 @@
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Buildarr.
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
-Dummy plugin configuration.
+Buildarr global runtime state.
 """
 
 
 from __future__ import annotations
 
-from pathlib import Path
-from typing import TYPE_CHECKING, Dict, Optional
-
-from typing_extensions import Self
+import os
 
-from buildarr.config import ConfigPlugin
-from buildarr.types import NonEmptyStr, Port
-
-from ..api import api_get
-from ..secrets import DummySecrets
-from ..types import DummyApiKey, DummyProtocol
-from .settings import DummySettingsConfig
+from collections import defaultdict
+from contextlib import contextmanager
+from distutils.util import strtobool
+from pathlib import Path
+from typing import TYPE_CHECKING, Tuple
 
-# Allow Mypy to properly resolve secrets type declarations in configuration classes.
 if TYPE_CHECKING:
+    from typing import DefaultDict, FrozenSet, Generator, Mapping, Optional, Sequence, Set
 
-    class _DummyInstanceConfig(ConfigPlugin[DummySecrets]):
-        ...
+    from .config import ConfigPlugin, ConfigType
+    from .manager import ManagerPlugin
+    from .plugins import Plugin
+    from .secrets import SecretsPlugin, SecretsType
 
-else:
 
-    class _DummyInstanceConfig(ConfigPlugin):
-        ...
+__all__ = ["state"]
 
+PluginInstanceRef = Tuple[str, str]
+"""
+A type for plugin-instance references as used in Buildarr internal state.
 
-class DummyInstanceConfig(_DummyInstanceConfig):
-    """
-    By default, Buildarr will look for a single instance at `http://dummy:5000`.
-    Most configurations are different, and to accommodate those, you can configure
-    how Buildarr connects to individual Dummy instances.
-
-    Configuration of a single Dummy instance:
+The first string in the tuple is the plugin name, and the second string is the instance name.
+"""
 
-    ```yaml
-    dummy:
-      hostname: "localhost"
-      port: 5000
-      protocol: "http"
-      settings:
-        ...
-    ```
 
-    Configuration of multiple instances:
+class State:
+    """
+    Active Buildarr state tracking class.
 
-    ```yaml
-    dummy:
-      # Configuration and settings common to all instances.
-      hostname: "localhost"
-      protocol: "http"
-      settings:
-        ...
-      instances:
-        # Dummy instance 1-specific configuration.
-        dummy1:
-          port: 5000
-          settings:
-            ...
-        # Dummy instance 2-specific configuration.
-        dummy:
-          port: 5001
-          api_key: "..." # Explicitly define API key
-          settings:
-            ...
-    ```
+    If anything needs to be shared between plugins or different parts of Buildarr
+    over the life of an update run, generally it goes here.
     """
 
-    hostname: NonEmptyStr = "dummy"  # type: ignore[assignment]
+    testing: bool = bool(strtobool(os.environ.get("BUILDARR_TESTING", "false")))
+    """
+    Whether Buildarr is in testing mode or not.
     """
-    Hostname of the Dummy instance to connect to.
 
-    When defining a single instance using the global `dummy` configuration block,
-    the default hostname is `dummy`.
+    dry_run: bool = False
+    """
+    Whether Buildarr is in dry run mode or not.
 
-    When using multiple instance-specific configurations, the default hostname
-    is the name given to the instance in the `instances` attribute.
+    When set to `True` under a CLI command that supports it, the command should not
+    perform any action that would change the state of any external instances.
 
-    ```yaml
-    dummy:
-      instances:
-        dummy1: # <--- This becomes the default hostname
-          ...
-    ```
+    Custom CLI commands can set this attribute to `True` if they support a dry-run mode.
     """
 
-    port: Port = 5000  # type: ignore[assignment]
+    plugins: Mapping[str, Plugin] = {}
     """
-    Port number of the Dummy instance to connect to.
+    The loaded Buildarr plugins, mapped to the plugin's unique name.
     """
 
-    protocol: DummyProtocol = "http"  # type: ignore[assignment]
+    config: ConfigType = None  # type: ignore[assignment]
     """
-    Communication protocol to use to connect to Dummy.
-
-    Values:
+    Currently loaded global configuration.
 
-    * `http`
+    This includes Buildarr configuration and configuration for enabled plugins.
     """
 
-    api_key: Optional[DummyApiKey] = None
+    config_files: Sequence[Path] = []
     """
-    API key to use to authenticate with the Dummy instance.
-
-    If undefined or set to `None`, automatically retrieve the API key.
-    This can only be done on Dummy instances with authentication disabled.
+    Currently loaded configuration files, in the order they were loaded.
     """
 
-    version: Optional[str] = None
+    managers: Mapping[str, ManagerPlugin[ConfigPlugin, SecretsPlugin]]
     """
-    The expected version of the Dummy instance.
-    If undefined or set to `None`, the version is auto-detected.
-
-    At the moment this attribute is unused, and there is likely no need to explicitly set it.
+    Manager objects for each currently loaded plugin.
     """
 
-    settings: DummySettingsConfig = DummySettingsConfig()
+    instance_configs: Mapping[str, Mapping[str, ConfigPlugin]]
     """
-    Dummy settings.
-    Configuration options for Dummy itself are set within this structure.
+    Fully qualified configuration objects for each instance, under each plugin.
     """
 
-    @property
-    def uses_trash_metadata(self) -> bool:
-        """
-        A flag determining whether or not this instance configuration uses TRaSH-Guides metadata.
-
-        Returns:
-            `True` if TRaSH-Guides metadata is used, otherwise `False`
-        """
-        return self.settings.uses_trash_metadata
+    active_plugins: FrozenSet[str]
+    """
+    A data structure containing the names of all the currently active plugins.
+    """
 
-    def render_trash_metadata(self, trash_metadata_dir: Path) -> Self:
-        """
-        Read TRaSH-Guides metadata, and return a configuration object with all templates rendered.
+    trash_metadata_dir: Path
+    """
+    TRaSH-Guides metadata directory.
 
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
+    Only available if required by at least one instance configuration,
+    during the render stage of a Buildarr run.
+    """
 
-        Returns:
-            Rendered configuration object
-        """
-        copy = self.copy(deep=True)
-        copy._render_trash_metadata(trash_metadata_dir)
-        return copy
+    secrets: SecretsType
+    """
+    Currently loaded instance secrets.
+    """
 
-    def _render_trash_metadata(self, trash_metadata_dir: Path) -> None:
-        """
-        Render configuration attributes obtained from TRaSH-Guides, in-place.
+    _current_dir: Path = Path.cwd()
+    """
+    Current working directory for relative path resolution.
 
-        Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
-        """
-        if self.settings.uses_trash_metadata:
-            self.settings._render_trash_metadata(trash_metadata_dir)
+    This state attribute is internal, and shouldn't be accessed by plugins.
+    """
 
-    @classmethod
-    def from_remote(cls, secrets: DummySecrets) -> Self:
-        """
-        Read configuration from a remote instance and return it as a configuration object.
+    _current_plugin: str
+    """
+    The plugin being processed in the current context.
 
-        Args:
-            secrets (DummySecrets): Instance host and secrets information
+    This state attribute is internal, and shouldn't be accessed by plugins.
+    """
 
-        Returns:
-            Configuration object for remote instance
-        """
-        return cls(
-            hostname=secrets.hostname,
-            port=secrets.port,
-            protocol=secrets.protocol,
-            api_key=secrets.api_key,
-            version=api_get(secrets, "/api/v1/status")["version"],
-            settings=DummySettingsConfig.from_remote(secrets),
-        )
+    _current_instance: str
+    """
+    The current instance being processed in the current context.
 
+    This state attribute is internal, and shouldn't be accessed by plugins.
+    """
 
-class DummyConfig(DummyInstanceConfig):
+    _instance_dependencies: DefaultDict[
+        PluginInstanceRef,  # source_plugin_instance
+        Set[PluginInstanceRef],  # target_plugin_instances
+    ]
     """
-    Dummy plugin global configuration class.
+    The dependency tree for linked instances defined in the Buildarr configuration.
+
+    This attribute is populated when instance name references get validated
+    upon fetching instance-specific configurations.
 
-    Subclasses the instance-specific configuration to allow
-    attributes common to all instances to be defined in one place.
+    This state attribute is internal, and shouldn't be accessed by plugins.
     """
 
-    instances: Dict[str, DummyInstanceConfig] = {}
+    _execution_order: Sequence[PluginInstanceRef]
     """
-    Instance-specific Dummy configuration.
+    A list of plugin-instance references in the order which operations
+    should be performed on them.
 
-    Can only be defined on the global `dummy` configuration block.
+    This attribute is generated based on the dependency tree for linked instances,
+    after `state._instance_dependencies` has finished being populated.
 
-    Globally specified configuration values apply to all instances.
-    Configuration values specified on an instance-level take precedence at runtime.
+    This state attribute is internal, and shouldn't be accessed by plugins.
     """
 
-    @property
-    def uses_trash_metadata(self) -> bool:
+    def __init__(self) -> None:
+        self._reset()
+
+    def _reset(self) -> None:
         """
-        A flag determining whether or not this configuration uses TRaSH-Guides metadata.
+        Reset the runtime state generated during an individual Buildarr run.
+
+        This is called in daemon mode to clean up after runs.
 
-        Returns:
-            `True` if TRaSH-Guides metadata is used, otherwise `False`
+        This state function is internal, and shouldn't be used by plugins.
         """
-        for instance in self.instances.values():
-            if instance.uses_trash_metadata:
-                return True
-        return super().uses_trash_metadata
+        self.managers = None  # type: ignore[assignment]
+        self.instance_configs = None  # type: ignore[assignment]
+        self.active_plugins = None  # type: ignore[assignment]
+        self.trash_metadata_dir = None  # type: ignore[assignment]
+        self.secrets = None  # type: ignore[assignment]
+        self._current_plugin = None  # type: ignore[assignment]
+        self._current_instance = None  # type: ignore[assignment]
+        self._instance_dependencies = defaultdict(set)  # type: ignore[assignment]
+        self._execution_order = None  # type: ignore[assignment]
 
-    def render_trash_metadata(self, trash_metadata_dir: Path) -> Self:
+    @contextmanager
+    def _with_current_dir(self, current_dir: Path) -> Generator[None, None, None]:
         """
-        Read TRaSH-Guides metadata, and return a configuration object with all templates rendered.
+        Set the current directory context within a code block.
+
+        This state function is internal, and shouldn't be used by plugins.
 
         Args:
-            trash_metadata_dir (Path): TRaSH-Guides metadata directory.
+            current_dir (Path): Path to use as the current directory.
+        """
+        old_current_dir = self._current_dir
+        self._current_dir = current_dir
+        yield
+        self._current_dir = old_current_dir
+
+    @contextmanager
+    def _with_context(
+        self,
+        plugin_name: Optional[str] = None,
+        instance_name: Optional[str] = None,
+    ) -> Generator[None, None, None]:
+        """
+        Set the current plugin/instance context within a code block.
+
+        This state function is internal, and shouldn't be used by plugins.
 
-        Returns:
-            Rendered configuration object
+        Args:
+            plugin_name (Optional[str], optional): Plugin name to set in the context.
+            instance_name (Optional[str], optional): Instance name to set in the context.
         """
-        copy = self.copy(deep=True)
-        for instance in copy.instances.values():
-            if instance.uses_trash_metadata:
-                instance._render_trash_metadata(trash_metadata_dir)
-        if self.uses_trash_metadata:
-            copy._render_trash_metadata(trash_metadata_dir)
-        return copy
+        if plugin_name:
+            old_current_plugin = self._current_plugin
+            self._current_plugin = plugin_name
+        if instance_name:
+            old_current_instance = self._current_instance
+            self._current_instance = instance_name
+        yield
+        if plugin_name:
+            self._current_plugin = old_current_plugin
+        if instance_name:
+            self._current_instance = old_current_instance
+
+
+state = State()
+"""
+Global variable for tracking active Buildarr state.
+
+If anything needs to be shared between plugins or different parts of Buildarr
+over the life of an update run, generally it goes here.
+"""
```

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/config/settings.py` & `buildarr-0.4.2/buildarr/plugins/dummy/config/settings.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/config/types.py` & `buildarr-0.4.2/buildarr/plugins/dummy/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/exceptions.py` & `buildarr-0.4.2/buildarr/plugins/dummy/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/manager.py` & `buildarr-0.4.2/buildarr/plugins/dummy/manager.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/plugin.py` & `buildarr-0.4.2/buildarr/plugins/dummy/plugin.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/secrets.py` & `buildarr-0.4.2/buildarr/plugins/dummy/secrets.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/server.py` & `buildarr-0.4.2/buildarr/plugins/dummy/server.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/dummy/types.py` & `buildarr-0.4.2/buildarr/plugins/dummy/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/load.py` & `buildarr-0.4.2/buildarr/plugins/load.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/models.py` & `buildarr-0.4.2/buildarr/plugins/models.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/plugins/types.py` & `buildarr-0.4.2/buildarr/plugins/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/secrets/__init__.py` & `buildarr-0.4.2/buildarr/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/secrets/base.py` & `buildarr-0.4.2/buildarr/secrets/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 """
 
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Generic
 
-from pydantic import BaseModel, SecretStr
+from pydantic import BaseModel
 
 from ..plugins import Config
+from ..types import ModelConfigBase
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from typing_extensions import Self
 
 
@@ -56,11 +57,41 @@
         Serialise the secrets metadata object and write it to a JSON file.
 
         Args:
             path (Path): Secrets JSON file to write to
         """
         path.write_text(self.json())
 
-    class Config:
-        json_encoders = {SecretStr: lambda v: v.get_secret_value()}
-        validate_all = True
+    class Config(ModelConfigBase):
+        """
+        Buildarr secrets model class settings.
+
+        Sets some required parameters for serialisation,
+        parsing and validation to work correctly.
+
+        To set additional parameters in your implementing class, subclass this class:
+
+        ```python
+        from __future__ import annotations
+
+        from typing import TYPE_CHECKING
+        from buildarr.secrets import SecretsBase
+
+        if TYPE_CHECKING:
+            from .config import ExampleConfig
+            class _ExampleSecrets(SecretsBase[ExampleSecrets]):
+                ...
+        else:
+            class _ExampleSecrets(SecretsBase):
+                ...
+
+        class ExampleSecrets(_ExampleSecrets):
+            ...
+
+            class Config(_ExampleSecrets.Config):
+                ...  # Add model configuration attributes here.
+        ```
+        """
+
+        # Validate any values that have been modified in-place, to ensure the model
+        # still fits the constraints.
         validate_assignment = True
```

### Comparing `buildarr-0.4.1/buildarr/secrets/load.py` & `buildarr-0.4.2/buildarr/secrets/load.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/secrets/models.py` & `buildarr-0.4.2/buildarr/secrets/models.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/buildarr/trash.py` & `buildarr-0.4.2/buildarr/trash.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 Buildarr TRaSH-Guides metadata functions.
 """
 
 
 from __future__ import annotations
 
 from collections import defaultdict
+from contextlib import contextmanager
 from logging import getLogger
 from pathlib import Path
-from shutil import move
+from shutil import move, rmtree
 from typing import TYPE_CHECKING
 from urllib.request import urlretrieve
 from zipfile import ZipFile
 
 from .state import state
 from .util import create_temp_dir
 
 if TYPE_CHECKING:
-    from typing import DefaultDict, Dict
+    from typing import DefaultDict, Dict, Generator
 
     from .config import ConfigPlugin
 
 
 logger = getLogger(__name__)
 
 
@@ -53,46 +54,60 @@
             with state._with_context(plugin_name=plugin_name, instance_name=instance_name):
                 if state.managers[plugin_name].uses_trash_metadata(instance_config):
                     return True
 
     return False
 
 
-def fetch_trash_metadata(trash_metadata_dir: Path) -> None:
+@contextmanager
+def fetch_trash_metadata() -> Generator[Path, None, None]:
     """
     Download the TRaSH-Guides metadata from the URL specified in the Buildarr config
-    to the given local directory.
+    to a temporary directory.
 
-    Args:
-        metadata_dir (Path): The local folder to extract the metadata to.
+    The temporary path gets added to the Buildarr global state, in addition to
+    being yielded to the caller.
+
+    Yields:
+        The temporary folder containing TRaSH-Guides metadata
     """
 
     logger.debug("Creating TRaSH metadata download temporary directory")
     with create_temp_dir() as temp_dir:
         logger.debug("Finished creating TRaSH metadata download temporary directory")
 
         trash_metadata_filename = temp_dir / "trash-metadata.zip"
 
         logger.debug("Downloading TRaSH metadata")
-        urlretrieve(state.config.buildarr.trash_metadata_download_url, trash_metadata_filename)
+        urlretrieve(  # noqa: S310  # `trash_metadata_download_url` is constrained to HTTP URLs.
+            state.config.buildarr.trash_metadata_download_url,
+            trash_metadata_filename,
+        )
         logger.debug("Finished downloading TRaSH metadata")
 
         logger.debug("Extracting TRaSH metadata")
         with ZipFile(trash_metadata_filename) as zip_file:
-            zip_file.extractall(path=temp_dir / "trash-metadata")
+            zip_file.extractall(path=temp_dir / "__trash-metadata__")
+        trash_metadata_filename.unlink()
         logger.debug("Finished extracting TRaSH metadata")
 
         logger.debug("Moving TRaSH metadata files to target directory")
         for subfile in (
-            temp_dir / "trash-metadata" / state.config.buildarr.trash_metadata_dir_prefix
+            temp_dir / "__trash-metadata__" / state.config.buildarr.trash_metadata_dir_prefix
         ).iterdir():
-            move(str(subfile), trash_metadata_dir)
+            move(str(subfile), temp_dir)
+        rmtree(temp_dir / "__trash-metadata__")
         logger.debug("Finished moving TRaSH metadata files to target directory")
 
-        # Temporary directory will be deleted when the with block is exited.
+        state.trash_metadata_dir = temp_dir
+        yield temp_dir
+        state.trash_metadata_dir = None  # type: ignore[assignment]
+
+        logger.debug("Deleting TRaSH metadata download temporary directory")
+    logger.debug("Finished deleting TRaSH metadata download temporary directory")
 
 
 def render_trash_metadata(trash_metadata_dir: Path) -> None:
     """
     Render TRaSH-Guides metadata on any instance configurations where used,
     and update the global state.
```

### Comparing `buildarr-0.4.1/buildarr/types.py` & `buildarr-0.4.2/buildarr/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,26 +16,31 @@
 Buildarr general purpose type hints, used in plugin models.
 """
 
 
 from __future__ import annotations
 
 import re
+import warnings
 
 from enum import Enum, IntEnum
-from pathlib import Path
-from typing import Any, Callable, Generator
+from pathlib import Path, PurePosixPath, PureWindowsPath
+from typing import TYPE_CHECKING, Any, Callable, Generator, Mapping
 
 from pydantic import AnyUrl, ConstrainedInt, ConstrainedStr, Field, SecretStr
 from pydantic.fields import ModelField
 from typing_extensions import Annotated, Self
 
 from .state import state
 from .util import get_absolute_path
 
+if TYPE_CHECKING:
+    from .config.models import ConfigPlugin
+
+
 Password = Annotated[SecretStr, Field(min_length=1)]
 """
 Constrained secrets string type for password fields. Required to be non-empty.
 """
 
 
 class RssUrl(AnyUrl):
@@ -231,14 +236,22 @@
 
         Raises:
             KeyError: When the enumeration name is invalid (does not exist).
 
         Returns:
             The enumeration object for the given name
         """
+        warnings.warn(
+            (
+                "BaseIntEnum is deprecated, and will be removed in Buildarr version 0.5.0. "
+                "Please update your Buildarr plugin to use BaseEnum instead."
+            ),
+            DeprecationWarning,
+            stacklevel=1,
+        )
         name = name_str.lower().replace("-", "_")
         for obj in cls:
             if obj.name.lower() == name:
                 return obj
         raise KeyError(repr(name))
 
     def to_name_str(self) -> str:
@@ -362,16 +375,14 @@
 
     @classmethod
     def validate(cls, value: str, field: ModelField) -> Self:
         """
         Validate the type of the instance name reference,
         evaluate the reference and add the link to the dependency tree structure.
 
-        _extended_summary_
-
         Args:
             value (str): Instance name reference.
             field (ModelField): Field metadata. Used to get the linked plugin name.
 
         Raises:
             ValueError: If the target plugin is not defined as field metadata
 
@@ -381,17 +392,30 @@
         NonEmptyStr.validate(value)
         try:
             plugin_name: str = field.field_info.extra["plugin"]
             instance_name = value
             if plugin_name not in state.plugins:
                 raise ValueError(f"Target plugin '{plugin_name}' not installed")
             if state.config:
-                if instance_name not in getattr(state.config, plugin_name).instances:
+                instances: Mapping[str, ConfigPlugin] = getattr(
+                    state.config,
+                    plugin_name,
+                ).instances
+                if instance_name == "default":
+                    if instances:
+                        raise ValueError(
+                            "unable to use default instance as the target instance, "
+                            "instance-specific configurations are defined "
+                            f"in plugin '{plugin_name}' configuration ("
+                            f"available instances: {', '.join(repr(i) for i in instances.keys())}"
+                            ")",
+                        )
+                elif instance_name not in instances:
                     raise ValueError(
-                        f"Target instance '{instance_name}' "
+                        f"target instance '{instance_name}' "
                         f"not defined in plugin '{plugin_name}' configuration",
                     )
                 if state._current_plugin and state._current_instance:
                     state._instance_dependencies[
                         (state._current_plugin, state._current_instance)
                     ].add(
                         (plugin_name, instance_name),
@@ -450,7 +474,43 @@
         Returns:
             Absolute local path
         """
         path = cls(value)
         if not path.is_absolute():
             return cls(get_absolute_path(state._current_dir / path))
         return path
+
+
+class ModelConfigBase:
+    """
+    Buildarr model configuration base class.
+
+    Sets some required configuration parameters for
+    serialisation, parsing and validation to work correctly.
+    """
+
+    # Add default JSON encoders for custom, non-default and otherwise non-specified
+    # classes so serialisation can work.
+    # Note that subclasses of types already handled by Python's built-in JSON encoder
+    # will *not* be read using this structure, so there are limitations as to
+    # what will work when defined here.
+    json_encoders = {
+        BaseEnum: lambda v: v.to_name_str(),
+        PurePosixPath: str,
+        PureWindowsPath: str,
+        SecretStr: lambda v: v.get_secret_value(),
+    }
+
+    # Required to avoid coersion with same-name but different-typed fields
+    # in objects for which there are multiple types that can be defined.
+    smart_union = True
+
+    # When aliases are defined, allow attributes to be referenced by their
+    # internal name, as well as the alias.
+    allow_population_by_field_name = True
+
+    # Validate all configuration attributes, even the default ones.
+    # This is necessary because the default attributes sometimes need to
+    # be validated for correctness in non-default contexts.
+    # (For example, a normally optional attribute becoming required due to
+    # another attribute being enabled.)
+    validate_all = True
```

### Comparing `buildarr-0.4.1/buildarr/util.py` & `buildarr-0.4.2/buildarr/util.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.1/pyproject.toml` & `buildarr-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "buildarr"
-version = "0.4.1"
+version = "0.4.2"
 description = "Constructs and configures Arr PVR stacks"
 authors = ["Callum Dickinson <callum.dickinson.nz@gmail.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://buildarr.github.io"
 repository = "https://github.com/buildarr/buildarr"
 documentation = "https://buildarr.github.io"
 keywords = ["buildarr", "sonarr", "radarr", "prowlarr"]
@@ -44,23 +44,23 @@
 click = ">=8.0.4"
 click-params = ">=0.4.1"
 watchdog = ">=3.0.0"
 schedule = ">=1.1.0"
 importlib-metadata = ">=4.6.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "23.1.0"
-mypy = "1.1.1"
-types-pyyaml = "6.0.12.8"
-types-requests = "2.28.11.15"
+black = "23.3.0"
+mypy = "1.2.0"
+types-pyyaml = "6.0.12.9"
+types-requests = "2.28.11.17"
 mkdocs = "1.4.2"
-mkdocstrings = {extras = ["python"], version = "0.20.0"}
+mkdocstrings = {extras = ["python"], version = "0.21.2"}
 flask = "2.2.3"
 werkzeug = "2.2.3"
-ruff = "0.0.255"
+ruff = "0.0.261"
 
 [tool.ruff]
 fix = true
 format = "grouped"
 target-version = "py38"
 line-length = 100
 select = [
```

### Comparing `buildarr-0.4.1/PKG-INFO` & `buildarr-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildarr
-Version: 0.4.1
+Version: 0.4.2
 Summary: Constructs and configures Arr PVR stacks
 Home-page: https://buildarr.github.io
 License: GPL-3.0-or-later
 Keywords: buildarr,sonarr,radarr,prowlarr
 Author: Callum Dickinson
 Author-email: callum.dickinson.nz@gmail.com
 Requires-Python: >=3.8,<4.0
```

