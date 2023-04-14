# Comparing `tmp/pipen-0.9.1.tar.gz` & `tmp/pipen-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen-0.9.1.tar", max compression
+gzip compressed data, was "pipen-0.9.2.tar", max compression
```

## Comparing `pipen-0.9.1.tar` & `pipen-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-04-14 01:51:06.416629 pipen-0.9.1/LICENSE
--rw-r--r--   0        0        0     9390 2023-04-14 01:51:06.416629 pipen-0.9.1/README.md
--rw-r--r--   0        0        0      318 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/__init__.py
--rw-r--r--   0        0        0       68 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/__main__.py
--rw-r--r--   0        0        0     7143 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/_job_caching.py
--rw-r--r--   0        0        0     6434 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/channel.py
--rw-r--r--   0        0        0       83 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/cli/__init__.py
--rw-r--r--   0        0        0      912 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/cli/_hooks.py
--rw-r--r--   0        0        0     1651 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/cli/_main.py
--rw-r--r--   0        0        0      973 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/cli/help.py
--rw-r--r--   0        0        0     3701 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/cli/plugins.py
--rw-r--r--   0        0        0     2906 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/cli/profile.py
--rw-r--r--   0        0        0     1181 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/cli/version.py
--rw-r--r--   0        0        0     2709 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/defaults.py
--rw-r--r--   0        0        0     1832 2023-04-14 01:51:06.420629 pipen-0.9.1/pipen/exceptions.py
--rw-r--r--   0        0        0     9499 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/job.py
--rw-r--r--   0        0        0    16596 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/pipen.py
--rw-r--r--   0        0        0     9965 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/pluginmgr.py
--rw-r--r--   0        0        0    23466 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/proc.py
--rw-r--r--   0        0        0     5489 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/procgroup.py
--rw-r--r--   0        0        0     4067 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/progressbar.py
--rw-r--r--   0        0        0     2404 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/scheduler.py
--rw-r--r--   0        0        0     3668 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/template.py
--rw-r--r--   0        0        0    14380 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/utils.py
--rw-r--r--   0        0        0       54 2023-04-14 01:51:06.424629 pipen-0.9.1/pipen/version.py
--rw-r--r--   0        0        0     1644 2023-04-14 01:51:06.424629 pipen-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    10494 1970-01-01 00:00:00.000000 pipen-0.9.1/setup.py
--rw-r--r--   0        0        0    10314 1970-01-01 00:00:00.000000 pipen-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 06:12:33.272959 pipen-0.9.2/LICENSE
+-rw-r--r--   0        0        0     9390 2023-04-14 06:12:33.272959 pipen-0.9.2/README.md
+-rw-r--r--   0        0        0      318 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/__init__.py
+-rw-r--r--   0        0        0       68 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/__main__.py
+-rw-r--r--   0        0        0     7143 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/_job_caching.py
+-rw-r--r--   0        0        0     6434 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/channel.py
+-rw-r--r--   0        0        0       83 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/__init__.py
+-rw-r--r--   0        0        0      912 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/_hooks.py
+-rw-r--r--   0        0        0     1651 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/_main.py
+-rw-r--r--   0        0        0      973 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/help.py
+-rw-r--r--   0        0        0     3701 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/plugins.py
+-rw-r--r--   0        0        0     2906 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/profile.py
+-rw-r--r--   0        0        0     1181 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/version.py
+-rw-r--r--   0        0        0     2709 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/defaults.py
+-rw-r--r--   0        0        0     1832 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/exceptions.py
+-rw-r--r--   0        0        0     9499 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/job.py
+-rw-r--r--   0        0        0    15070 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/pipen.py
+-rw-r--r--   0        0        0     9965 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/pluginmgr.py
+-rw-r--r--   0        0        0    23466 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/proc.py
+-rw-r--r--   0        0        0     5489 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/procgroup.py
+-rw-r--r--   0        0        0     4066 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/progressbar.py
+-rw-r--r--   0        0        0     2404 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/scheduler.py
+-rw-r--r--   0        0        0     3668 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/template.py
+-rw-r--r--   0        0        0    14380 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/utils.py
+-rw-r--r--   0        0        0       54 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/version.py
+-rw-r--r--   0        0        0     1644 2023-04-14 06:12:33.276959 pipen-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10494 1970-01-01 00:00:00.000000 pipen-0.9.2/setup.py
+-rw-r--r--   0        0        0    10314 1970-01-01 00:00:00.000000 pipen-0.9.2/PKG-INFO
```

### Comparing `pipen-0.9.1/LICENSE` & `pipen-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/README.md` & `pipen-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/_job_caching.py` & `pipen-0.9.2/pipen/_job_caching.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/channel.py` & `pipen-0.9.2/pipen/channel.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/cli/_hooks.py` & `pipen-0.9.2/pipen/cli/_hooks.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/cli/_main.py` & `pipen-0.9.2/pipen/cli/_main.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/cli/help.py` & `pipen-0.9.2/pipen/cli/help.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/cli/plugins.py` & `pipen-0.9.2/pipen/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/cli/profile.py` & `pipen-0.9.2/pipen/cli/profile.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/cli/version.py` & `pipen-0.9.2/pipen/cli/version.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/defaults.py` & `pipen-0.9.2/pipen/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Remove the rich handler
 _xqute_handlers = xqute_logger.handlers
 if _xqute_handlers:
     # The very first handler is the rich handler
     xqute_logger.removeHandler(_xqute_handlers[0])
 
-LOGGER_NAME = "main"
+LOGGER_NAME = "core"
 CONFIG_FILES = (
     Path("~/.pipen.toml").expanduser(),
     "./.pipen.toml",
     "PIPEN.osenv",
 )
 CONFIG = Diot(
     # pipeline level: The logging level
```

### Comparing `pipen-0.9.1/pipen/exceptions.py` & `pipen-0.9.2/pipen/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/job.py` & `pipen-0.9.2/pipen/job.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/pipen.py` & `pipen-0.9.2/pipen/pipen.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """Main entry module, provide the Pipen class"""
 from __future__ import annotations
 
 import asyncio
-from itertools import chain
 from os import PathLike
 from pathlib import Path
-import pprint
-import textwrap
 from typing import Any, ClassVar, Iterable, List, Sequence, Type
 
 from diot import Diot
 from rich import box
 from rich.panel import Panel
-from rich.table import Table
 from rich.text import Text
-from rich.console import Group
 from simpleconf import ProfileConfig
 from varname import varname, VarnameException
 
 from .defaults import CONFIG, CONFIG_FILES
 from .exceptions import (
     PipenOrProcNameError,
     ProcDependencyError,
@@ -94,27 +89,22 @@
             try:
                 self.name = varname()
             except VarnameException:
                 self.name = f"pipen-{self.__class__.PIPELINE_COUNT}"
 
         if not is_valid_name(self.name):
             raise PipenOrProcNameError(
-                f"Invalid pipeline name: {self.name}, "
-                r"expecting '^[\w.-]$'"
+                fr"Invalid pipeline name: {self.name}, expecting '^[\w.-]$'"
             )
 
         self.desc = (
-            desc
-            or self.__class__.desc
-            or desc_from_docstring(self.__class__)
+            desc or self.__class__.desc or desc_from_docstring(self.__class__)
         )
         self.outdir = Path(
-            outdir
-            or self.__class__.outdir
-            or f"./{self.name}_results"
+            outdir or self.__class__.outdir or f"./{self.name}_results"
         ).resolve()
         self.workdir: Path = None
         self.profile: str = "default"
 
         self.starts: List[Proc] = self.__class__.starts
         if self.starts and not isinstance(self.starts, (tuple, list)):
             self.starts = [self.starts]
@@ -148,16 +138,16 @@
             # cyclic imports
             plugin.load_entrypoints()
 
         plugins = self.config.plugins or self._kwargs.get("plugins", [])
         self.plugin_context = get_plugin_context(plugins)
         self.plugin_context.__enter__()
 
-        # make sure main plugin is enabled
-        plugin.get_plugin("main").enable()
+        # make sure core plugin is enabled
+        plugin.get_plugin("core").enable()
 
         if not self.__class__.SETUP:  # pragma: no cover
             plugin.hooks.on_setup(self.config)
             self.__class__.SETUP = True
 
         self.__class__.PIPELINE_COUNT += 1
 
@@ -295,118 +285,60 @@
         return self
 
     # In case people forget the "s"
     set_start = set_starts
 
     def _log_pipeline_info(self) -> None:
         """Print the information of the pipeline"""
-        items = (
-            [
-                Panel(
-                    self.desc,
-                    box=box.Box(
-                        "    \n    \n    \n    \n    \n    \n    \n────\n",
-                    ),
-                    padding=(0, 0),
-                )
-            ]
-            if self.desc
-            else []
-        )
-
-        items_table = Table.grid(padding=(0, 1), pad_edge=True)
-        items.append(items_table)  # type: ignore
-        enabled_plugins = [
-            "{name}{version}".format(
-                name=name,
-                version=(f"-{plg.__version__}" if plg.version else ""),
-            )
-            for name, plg in plugin.get_enabled_plugins().items()
-        ]
-        config = ProfileConfig.detach(self.config)
-        for key, value in chain(
-            zip(
-                ["# procs", "plugins", "profile", "outdir"],
-                [
-                    str(len(self.procs)),
-                    enabled_plugins,
-                    self.profile,
-                    self.outdir,
-                ],
-            ),
-            sorted(
-                (key, val)
-                for key, val in config.items()
-                if not key.endswith("_opts")
-            ),
-            (
-                (
-                    "plugin_opts",
-                    pprint.pformat(config.plugin_opts, indent=1),
-                ),
-                (
-                    "scheduler_opts",
-                    pprint.pformat(config.scheduler_opts, indent=1),
-                ),
-                (
-                    "template_opts",
-                    pprint.pformat(
-                        {
-                            key: (
-                                {
-                                    ckey: textwrap.shorten(
-                                        str(cval),
-                                        width=30 - len(key),
-                                        placeholder=" …",
-                                    )
-                                    for ckey, cval in chain(
-                                        list(val.items())[:3],
-                                        []
-                                        if len(val) <= 3
-                                        else [("...", "...")],
-                                    )
-                                }
-                                if isinstance(val, dict)
-                                else val
-                            )
-                            for key, val in config.template_opts.items()
-                        },
-                        indent=1,
-                        # sort_dicts=False,
-                    ),
-                ),
-            ),
-        ):
-            items_table.add_row(
-                Text.assemble((key, "scope.key")),
-                Text.assemble(("=", "scope.equals")),
-                Text(str(value), overflow="fold"),
-            )
-
         logger.info("")
+        # Pipeline line and description
         log_rich_renderable(
             Panel(
-                Group(*items),
-                title=self.name.upper(),
+                self.desc or Text(self.name.upper(), justify="center"),
                 width=get_logpanel_width(),
-                box=box.Box(
-                    "╭═┬╮\n"
-                    "║ ║║\n"
-                    "├═┼┤\n"
-                    "║ ║║\n"
-                    "├═┼┤\n"
-                    "├═┼┤\n"
-                    "║ ║║\n"
-                    "╰═┴╯\n"
-                ),
-                padding=(0, 1),
+                # padding=(0, 1),
+                box=box.DOUBLE_EDGE,
+                title=self.name.upper() if self.desc else None,
             ),
-            None,
+            "magenta",
             logger.info,
         )
+        fmt = "[bold][magenta]%-16s:[/magenta][/bold] %s"
+        enabled_plugins = (
+            "{name} [cyan]{version}[/cyan]".format(
+                name=name,
+                version=(f"v{plg.version}" if plg.version else ""),
+            )
+            for name, plg in plugin.get_enabled_plugins().items()
+            if name != "core"
+        )
+        for i, plug in enumerate(enabled_plugins):
+            logger.info(fmt, "plugins" if i == 0 else "", plug)
+        logger.info(fmt, "# procs", len(self.procs))
+        logger.info(fmt, "profile", self.profile)
+        logger.info(fmt, "outdir", self.outdir)
+        logger.info(fmt, "cache", self.config.cache)
+        logger.info(fmt, "dirsig", self.config.dirsig)
+        logger.info(fmt, "error_strategy", self.config.error_strategy)
+        logger.info(fmt, "forks", self.config.forks)
+        logger.info(fmt, "lang", self.config.lang)
+        logger.info(fmt, "loglevel", self.config.loglevel)
+        logger.info(fmt, "num_retries", self.config.num_retries)
+        logger.info(fmt, "scheduler", self.config.scheduler)
+        logger.info(fmt, "submission_batch", self.config.submission_batch)
+        logger.info(fmt, "template", self.config.template)
+        logger.info(fmt, "workdir", self.config.workdir)
+        for i, (key, val) in enumerate(self.config.plugin_opts.items()):
+            logger.info(fmt, "plugin_opts" if i == 0 else "", f"{key}={val}")
+        for i, (key, val) in enumerate(self.config.scheduler_opts.items()):
+            logger.info(
+                fmt, "scheduler_opts" if i == 0 else "", f"{key}={val}"
+            )
+        for i, (key, val) in enumerate(self.config.template_opts.items()):
+            logger.info(fmt, "template_opts" if i == 0 else "", f"{key}={val}")
 
     async def _init(self) -> None:
         """Compute the configurations for the pipeline based on the priorities
 
         Configurations (priority from low to high)
         1. The default config in .defaults
         2. The plugin_opts defined in plugins (via on_setup() hook)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pipen-0.9.1/pipen/pluginmgr.py` & `pipen-0.9.2/pipen/pluginmgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,18 +231,18 @@
     Args:
         proc: The process
         job: The job
     """
 
 
 class PipenMainPlugin:
-    """The builtin main plugin, used to update the progress bar and
+    """The builtin core plugin, used to update the progress bar and
     cache the job"""
 
-    name = "main"
+    name = "core"
     # The priority is set to -1000 to make sure it is the first plugin
     # to be called
     order = -1000
 
     @plugin.impl
     def on_proc_shutdown(self, proc: Proc, sig: signal.Signals):
         """When a process is shutting down"""
```

### Comparing `pipen-0.9.1/pipen/proc.py` & `pipen-0.9.2/pipen/proc.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/procgroup.py` & `pipen-0.9.2/pipen/procgroup.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/progressbar.py` & `pipen-0.9.2/pipen/progressbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING
 
 from .utils import truncate_text
 
 if TYPE_CHECKING:  # pragma: no cover
     import enlighten
 
-# [12/02/20 12:44:06] I /main
+# [12/02/20 12:44:06] I core
 #                 pipeline: 100%|
 # |        desc_len      |
 PBAR_DESC_LEN = 23
 
 
 class ProcPBar:
     """The progress bar for processes"""
```

### Comparing `pipen-0.9.1/pipen/scheduler.py` & `pipen-0.9.2/pipen/scheduler.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/template.py` & `pipen-0.9.2/pipen/template.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pipen/utils.py` & `pipen-0.9.2/pipen/utils.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.1/pyproject.toml` & `pipen-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "pipen"
-version = "0.9.1"
+version = "0.9.2"
 description = "A pipeline framework for python"
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen"
 repository = "https://github.com/pwwang/pipen"
```

### Comparing `pipen-0.9.1/setup.py` & `pipen-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'xqute>=0.2.1,<0.3.0']
 
 entry_points = \
 {'console_scripts': ['pipen = pipen.cli:main']}
 
 setup_kwargs = {
     'name': 'pipen',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'A pipeline framework for python',
     'long_description': '<div align="center">\n    <img src="./pipen.png" width="320px">\n\n**A pipeline framework for python**\n\n</div>\n\n______________________________________________________________________\n\n[![Pypi][6]][7] [![Github][8]][9] ![Building][10] [![Docs and API][11]][1] [![Codacy][12]][13] [![Codacy coverage][14]][13] [![Deps][5]][23]\n\n[Documentation][1] | [ChangeLog][2] | [Examples][3] | [API][4]\n\n## Features\n\n- Easy to use\n- Nearly zero-configuration\n- Nice logging\n- Highly extendable\n\n## Installation\n\n```bash\npip install -U pipen\n```\n\n## Quickstart\n\n`example.py`\n\n```python\nfrom pipen import Proc, Pipen\n\nclass P1(Proc):\n    """Sort input file"""\n    input = "infile"\n    input_data = ["/tmp/data.txt"]\n    output = "outfile:file:intermediate.txt"\n    script = "cat {{in.infile}} | sort > {{out.outfile}}"\n\nclass P2(Proc):\n    """Paste line number"""\n    requires = P1\n    input = "infile"\n    output = "outfile:file:result.txt"\n    script = "paste <(seq 1 3) {{in.infile}} > {{out.outfile}}"\n\nclass MyPipeline(Pipen):\n    starts = P1\n\nif __name__ == "__main__":\n    MyPipeline().run()\n```\n\n```shell\n> echo -e "3\\n2\\n1" > /tmp/data.txt\n> python example.py\n```\n\n```log\n[09/13/21 04:23:37] I main                    _____________________________________   __\n[09/13/21 04:23:37] I main                    ___  __ \\___  _/__  __ \\__  ____/__  | / /\n[09/13/21 04:23:37] I main                    __  /_/ /__  / __  /_/ /_  __/  __   |/ /\n[09/13/21 04:23:37] I main                    _  ____/__/ /  _  ____/_  /___  _  /|  /\n[09/13/21 04:23:37] I main                    /_/     /___/  /_/     /_____/  /_/ |_/\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main                                 version: 0.9.0\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭═════════════════════════════ MYPIPELIN ═══════════════════════════════╮\n[09/13/21 04:23:37] I main    ║  # procs          = 2                                                 ║\n[09/13/21 04:23:37] I main    ║  plugins          = [\'main\', \'verbose-0.0.1\']                         ║\n[09/13/21 04:23:37] I main    ║  profile          = default                                           ║\n[09/13/21 04:23:37] I main    ║  outdir           = mypipeline_results                                ║\n[09/13/21 04:23:37] I main    ║  cache            = True                                              ║\n[09/13/21 04:23:37] I main    ║  dirsig           = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  error_strategy   = ignore                                            ║\n[09/13/21 04:23:37] I main    ║  forks            = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  lang             = bash                                              ║\n[09/13/21 04:23:37] I main    ║  loglevel         = info                                              ║\n[09/13/21 04:23:37] I main    ║  num_retries      = 3                                                 ║\n[09/13/21 04:23:37] I main    ║  plugin_opts      = {}                                                ║\n[09/13/21 04:23:37] I main    ║  plugins          = None                                              ║\n[09/13/21 04:23:37] I main    ║  scheduler        = local                                             ║\n[09/13/21 04:23:37] I main    ║  scheduler_opts   = {}                                                ║\n[09/13/21 04:23:37] I main    ║  submission_batch = 8                                                 ║\n[09/13/21 04:23:37] I main    ║  template         = liquid                                            ║\n[09/13/21 04:23:37] I main    ║  template_opts    = {}                                                ║\n[09/13/21 04:23:37] I main    ║  workdir          = ./.pipen                                          ║\n[09/13/21 04:23:37] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭───────────────────────────────── P1 ──────────────────────────────────╮\n[09/13/21 04:23:37] I main    │ Sort input file                                                       │\n[09/13/21 04:23:37] I main    ╰───────────────────────────────────────────────────────────────────────╯\n[09/13/21 04:23:37] I main    P1: Workdir: \'.pipen/mypipeline/p1\'\n[09/13/21 04:23:37] I main    P1: <<< [START]\n[09/13/21 04:23:37] I main    P1: >>> [\'P2\']\n[09/13/21 04:23:37] I verbose P1: size: 1\n[09/13/21 04:23:37] I verbose P1: [0/0] in.infile: /tmp/data.txt\n[09/13/21 04:23:37] I verbose P1: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P1: Time elapsed: 00:00:01.039s\n[09/13/21 04:23:38] I main\n[09/13/21 04:23:38] I main    ╭═════════════════════════════════ P2 ══════════════════════════════════╮\n[09/13/21 04:23:38] I main    ║ Paste line number                                                     ║\n[09/13/21 04:23:38] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:38] I main    P2: Workdir: \'.pipen/mypipeline/p2\'\n[09/13/21 04:23:38] I main    P2: <<< [\'P1\']\n[09/13/21 04:23:38] I main    P2: >>> [END]\n[09/13/21 04:23:38] I verbose P2: size: 1\n[09/13/21 04:23:38] I verbose P2: [0/0] in.infile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P2: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/mypipeline_results/P2/result.txt\n[09/13/21 04:23:40] I verbose P2: Time elapsed: 00:00:02.074s\n[09/13/21 04:23:40] I main\n\n                PIPEN-0: 100%|████████████████████████████████████████| 2/2 [00:04<00:00, 0.56 procs/s]\n```\n\n```shell\n> cat ./mypipeline_results/P2/result.txt\n1       1\n2       2\n3       3\n```\n\n## Examples\n\nSee more examples at `examples/` and a more realcase example at:\nhttps://github.com/pwwang/pipen-report/tree/master/example\n\n## Plugin gallery\n\nPlugins make `pipen` even better.\n\n- [`pipen-verbose`][15]: Add verbosal information in logs for pipen.\n- [`pipen-lock`][25]: Process lock for pipen to prevent multiple runs at the same time.\n- [`pipen-report`][16]: Generate report for pipen\n- [`pipen-filters`][17]: Add a set of useful filters for pipen templates.\n- [`pipen-diagram`][18]: Draw pipeline diagrams for pipen\n- [`pipen-annotate`][26]: Use docstring to annotate pipen processes\n- [`pipen-args`][19]: Command line argument parser for pipen\n- [`pipen-dry`][20]: Dry runner for pipen pipelines\n- [`pipen-cli-init`][21]: A pipen CLI plugin to create a pipen project (pipeline)\n- [`pipen-cli-run`][22]: A pipen cli plugin to run a process or a pipeline\n- [`pipen-cli-config`][27]: UI wizard to generate configuration for pipen pipelines\n- [`pipen-cli-require`][24]: A pipen cli plugin check the requirements of a pipeline\n\n\n[1]: https://pwwang.github.io/pipen\n[2]: https://pwwang.github.io/pipen/CHANGELOG\n[3]: https://pwwang.github.io/pipen/examples\n[4]: https://pwwang.github.io/pipen/api/pipen\n[5]: https://img.shields.io/librariesio/release/pypi/pipen?style=flat-square\n[6]: https://img.shields.io/pypi/v/pipen?style=flat-square\n[7]: https://pypi.org/project/pipen/\n[8]: https://img.shields.io/github/v/tag/pwwang/pipen?style=flat-square\n[9]: https://github.com/pwwang/pipen\n[10]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/build.yml?style=flat-square\n[11]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/docs.yml?label=docs&style=flat-square\n[12]: https://img.shields.io/codacy/grade/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[13]: https://app.codacy.com/gh/pwwang/pipen\n[14]: https://img.shields.io/codacy/coverage/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[15]: https://github.com/pwwang/pipen-verbose\n[16]: https://github.com/pwwang/pipen-report\n[17]: https://github.com/pwwang/pipen-filters\n[18]: https://github.com/pwwang/pipen-diagram\n[19]: https://github.com/pwwang/pipen-args\n[20]: https://github.com/pwwang/pipen-dry\n[21]: https://github.com/pwwang/pipen-cli-init\n[22]: https://github.com/pwwang/pipen-cli-run\n[23]: https://libraries.io/github/pwwang/pipen#repository_dependencies\n[24]: https://github.com/pwwang/pipen-cli-require\n[25]: https://github.com/pwwang/pipen-lock\n[26]: https://github.com/pwwang/pipen-annotate\n[27]: https://github.com/pwwang/pipen-cli-config\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen',
```

### Comparing `pipen-0.9.1/PKG-INFO` & `pipen-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen
-Version: 0.9.1
+Version: 0.9.2
 Summary: A pipeline framework for python
 Home-page: https://github.com/pwwang/pipen
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

