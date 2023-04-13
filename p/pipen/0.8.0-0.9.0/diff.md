# Comparing `tmp/pipen-0.8.0.tar.gz` & `tmp/pipen-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen-0.8.0.tar", max compression
+gzip compressed data, was "pipen-0.9.0.tar", max compression
```

## Comparing `pipen-0.8.0.tar` & `pipen-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-04-11 17:04:51.925708 pipen-0.8.0/LICENSE
--rw-r--r--   0        0        0     9390 2023-04-11 17:04:51.925708 pipen-0.8.0/README.md
--rw-r--r--   0        0        0      318 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/__init__.py
--rw-r--r--   0        0        0       68 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/__main__.py
--rw-r--r--   0        0        0     7143 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/_job_caching.py
--rw-r--r--   0        0        0     6434 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/channel.py
--rw-r--r--   0        0        0       83 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/__init__.py
--rw-r--r--   0        0        0      912 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/_hooks.py
--rw-r--r--   0        0        0     1651 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/_main.py
--rw-r--r--   0        0        0      973 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/help.py
--rw-r--r--   0        0        0     3701 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/plugins.py
--rw-r--r--   0        0        0     2906 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/profile.py
--rw-r--r--   0        0        0     1422 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/version.py
--rw-r--r--   0        0        0     2623 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/defaults.py
--rw-r--r--   0        0        0     1832 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/exceptions.py
--rw-r--r--   0        0        0     9478 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/job.py
--rw-r--r--   0        0        0    16597 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/pipen.py
--rw-r--r--   0        0        0     9965 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/pluginmgr.py
--rw-r--r--   0        0        0    23511 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/proc.py
--rw-r--r--   0        0        0     5507 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/procgroup.py
--rw-r--r--   0        0        0     4067 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/progressbar.py
--rw-r--r--   0        0        0     1857 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/scheduler.py
--rw-r--r--   0        0        0     3668 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/template.py
--rw-r--r--   0        0        0    14662 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/utils.py
--rw-r--r--   0        0        0       54 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/version.py
--rw-r--r--   0        0        0     1665 2023-04-11 17:04:51.933708 pipen-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    10516 1970-01-01 00:00:00.000000 pipen-0.8.0/setup.py
--rw-r--r--   0        0        0    10350 1970-01-01 00:00:00.000000 pipen-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 22:30:52.521522 pipen-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9390 2023-04-13 22:30:52.521522 pipen-0.9.0/README.md
+-rw-r--r--   0        0        0      318 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/__init__.py
+-rw-r--r--   0        0        0       68 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/__main__.py
+-rw-r--r--   0        0        0     7143 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/_job_caching.py
+-rw-r--r--   0        0        0     6434 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/channel.py
+-rw-r--r--   0        0        0       83 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/cli/__init__.py
+-rw-r--r--   0        0        0      912 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/cli/_hooks.py
+-rw-r--r--   0        0        0     1651 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/cli/_main.py
+-rw-r--r--   0        0        0      973 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/cli/help.py
+-rw-r--r--   0        0        0     3701 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/cli/plugins.py
+-rw-r--r--   0        0        0     2906 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/cli/profile.py
+-rw-r--r--   0        0        0     1181 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/cli/version.py
+-rw-r--r--   0        0        0     2475 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/defaults.py
+-rw-r--r--   0        0        0     1832 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/exceptions.py
+-rw-r--r--   0        0        0     9499 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/job.py
+-rw-r--r--   0        0        0    16596 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/pipen.py
+-rw-r--r--   0        0        0     9965 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/pluginmgr.py
+-rw-r--r--   0        0        0    23497 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/proc.py
+-rw-r--r--   0        0        0     5489 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/procgroup.py
+-rw-r--r--   0        0        0     4067 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/progressbar.py
+-rw-r--r--   0        0        0     2404 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/scheduler.py
+-rw-r--r--   0        0        0     3668 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/template.py
+-rw-r--r--   0        0        0    14380 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/utils.py
+-rw-r--r--   0        0        0       54 2023-04-13 22:30:52.525522 pipen-0.9.0/pipen/version.py
+-rw-r--r--   0        0        0     1642 2023-04-13 22:30:52.525522 pipen-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10490 1970-01-01 00:00:00.000000 pipen-0.9.0/setup.py
+-rw-r--r--   0        0        0    10310 1970-01-01 00:00:00.000000 pipen-0.9.0/PKG-INFO
```

### Comparing `pipen-0.8.0/LICENSE` & `pipen-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/README.md` & `pipen-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ```log
 [09/13/21 04:23:37] I main                    _____________________________________   __
 [09/13/21 04:23:37] I main                    ___  __ \___  _/__  __ \__  ____/__  | / /
 [09/13/21 04:23:37] I main                    __  /_/ /__  / __  /_/ /_  __/  __   |/ /
 [09/13/21 04:23:37] I main                    _  ____/__/ /  _  ____/_  /___  _  /|  /
 [09/13/21 04:23:37] I main                    /_/     /___/  /_/     /_____/  /_/ |_/
 [09/13/21 04:23:37] I main
-[09/13/21 04:23:37] I main                                 version: 0.7.0
+[09/13/21 04:23:37] I main                                 version: 0.9.0
 [09/13/21 04:23:37] I main
 [09/13/21 04:23:37] I main    ╭═════════════════════════════ MYPIPELIN ═══════════════════════════════╮
 [09/13/21 04:23:37] I main    ║  # procs          = 2                                                 ║
 [09/13/21 04:23:37] I main    ║  plugins          = ['main', 'verbose-0.0.1']                         ║
 [09/13/21 04:23:37] I main    ║  profile          = default                                           ║
 [09/13/21 04:23:37] I main    ║  outdir           = mypipeline_results                                ║
 [09/13/21 04:23:37] I main    ║  cache            = True                                              ║
```

### Comparing `pipen-0.8.0/pipen/_job_caching.py` & `pipen-0.9.0/pipen/_job_caching.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/channel.py` & `pipen-0.9.0/pipen/channel.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/cli/_hooks.py` & `pipen-0.9.0/pipen/cli/_hooks.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/cli/_main.py` & `pipen-0.9.0/pipen/cli/_main.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/cli/help.py` & `pipen-0.9.0/pipen/cli/help.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/cli/plugins.py` & `pipen-0.9.0/pipen/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/cli/profile.py` & `pipen-0.9.0/pipen/cli/profile.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/cli/version.py` & `pipen-0.9.0/pipen/cli/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,46 +8,38 @@
 
 if TYPE_CHECKING:
     from argparse import Namespace
 
 __all__ = ("CLIVersionPlugin",)
 
 
-def get_pkg_version(pkg: str) -> str:
-    try:
-        from importlib.metadata import version
-        return version(pkg)
-    except ImportError:  # pragma: no cover
-        from pkg_resources import get_distribution  # type: ignore
-        return get_distribution(pkg).version
-
-
 class CLIVersionPlugin(CLIPlugin):
     """Print versions of pipen and its dependencies"""
 
     name = "version"
 
     def exec_command(self, args: Namespace) -> None:
         """Run the command"""
         import sys
+        from importlib.metadata import version
         from .. import __version__
 
         versions = {"python": sys.version, "pipen": __version__}
 
         for pkg in (
             "liquidpy",
             "pandas",
             "enlighten",
             "argx",
             "xqute",
             "python-simpleconf",
             "pipda",
             "varname",
         ):
-            versions[pkg] = get_pkg_version(pkg)
+            versions[pkg] = version(pkg)
 
         keylen = max(map(len, versions))
         for key in versions:
             ver = versions[key]
             verlines = ver.splitlines()
             print(f"{key.ljust(keylen)}: {verlines.pop(0)}")
             for verline in verlines:  # pragma: no cover
```

### Comparing `pipen-0.8.0/pipen/defaults.py` & `pipen-0.9.0/pipen/defaults.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 """Provide some default values/objects"""
 from pathlib import Path
 from typing import ClassVar
 
 from diot import Diot
 from xqute import JobErrorStrategy
-from xqute import logger as xqute_logger
-
-# turn xqute's logger off
-xqute_logger.setLevel(100)
-xqute_logger.removeHandler(xqute_logger.handlers[0])
 
 LOGGER_NAME = "main"
 CONFIG_FILES = (
     Path("~/.pipen.toml").expanduser(),
     "./.pipen.toml",
     "PIPEN.osenv",
 )
```

### Comparing `pipen-0.8.0/pipen/exceptions.py` & `pipen-0.9.0/pipen/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/job.py` & `pipen-0.9.0/pipen/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Provide the Job class"""
 from __future__ import annotations
 
 import logging
 import shlex
+import shutil
+from functools import cached_property
 from os import PathLike
 from pathlib import Path
-import shutil
 from typing import TYPE_CHECKING, Any, Dict, Mapping
 
 from diot import OrderedDiot
 from xqute import Job as XquteJob
 from xqute.utils import a_read_text
 
 from ._job_caching import JobCaching
@@ -18,15 +19,15 @@
     ProcInputTypeError,
     ProcOutputNameError,
     ProcOutputTypeError,
     ProcOutputValueError,
     TemplateRenderingError,
 )
 from .template import Template
-from .utils import cached_property, logger, strsplit
+from .utils import logger, strsplit
 
 if TYPE_CHECKING:  # pragma: no cover
     from .proc import Proc
 
 
 class Job(XquteJob, JobCaching):
     """The job for pipen"""
```

### Comparing `pipen-0.8.0/pipen/pipen.py` & `pipen-0.9.0/pipen/pipen.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                 proc_obj = proc(self)  # type: ignore
                 if proc in self.starts and proc.input_data is None:
                     proc_obj.log(
                         "warning",
                         "This is a start process, "
                         "but no 'input_data' specified.",
                     )
-                await proc_obj._init()
+                await proc_obj.init()
                 await proc_obj.run()
                 if proc_obj.succeeded:
                     self.pbar.update_proc_done()
                 else:
                     self.pbar.update_proc_error()
                     succeeded = False
                     break
```

### Comparing `pipen-0.8.0/pipen/pluginmgr.py` & `pipen-0.9.0/pipen/pluginmgr.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/proc.py` & `pipen-0.9.0/pipen/proc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """Provides the process class: Proc"""
 from __future__ import annotations
 
 import asyncio
 import inspect
-from abc import ABC, ABCMeta
 import logging
+from abc import ABC, ABCMeta
+from functools import cached_property
 from os import PathLike
 from pathlib import Path
 from typing import (
     Any,
     Dict,
     List,
     Mapping,
     Sequence,
     Type,
     TYPE_CHECKING,
 )
 
-# Slow down the import, try do it at runtime
-# import pandas
 from diot import Diot
 from rich import box
 from rich.panel import Panel
 from varname import VarnameException, varname
 from xqute import JobStatus, Xqute
 
 from .defaults import ProcInputType
@@ -33,15 +32,14 @@
     PipenOrProcNameError,
 )
 from .pluginmgr import plugin
 from .scheduler import get_scheduler
 from .template import Template, get_template_engine
 from .utils import (
     brief_list,
-    cached_property,
     copy_dict,
     desc_from_docstring,
     get_logpanel_width,
     ignore_firstline_dedent,
     is_subclass,
     is_valid_name,
     log_rich_renderable,
@@ -364,25 +362,26 @@
         # script
         self.script = self._compute_script()  # type: ignore
         self.workdir.mkdir(exist_ok=True)
 
         if self.submission_batch is None:
             self.submission_batch = self.pipeline.config.submission_batch
 
-    async def _init(self) -> None:
+    async def init(self) -> None:
         """Init all other properties and jobs"""
         import pandas
 
         scheduler_opts = (
             copy_dict(self.pipeline.config.scheduler_opts, 2) or {}
         )
         scheduler_opts.update(self.scheduler_opts or {})
         self.xqute = Xqute(
             self.scheduler,
             job_metadir=self.workdir,
+            loglevel="NOTSET",
             job_submission_batch=self.submission_batch,
             job_error_strategy=self.error_strategy
             or self.pipeline.config.error_strategy,
             job_num_retries=self.pipeline.config.num_retries
             if self.num_retries is None
             else self.num_retries,
             scheduler_forks=self.forks or self.pipeline.config.forks,
```

### Comparing `pipen-0.8.0/pipen/procgroup.py` & `pipen-0.9.0/pipen/procgroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,20 +32,19 @@
 >>>             ...
 >>>         return MyProc
 >>> proc_group = MyProcGroup(...)
 """
 from __future__ import annotations
 
 from os import PathLike
-from functools import wraps
+from functools import wraps, cached_property
 from typing import Callable, Type, List
 from abc import ABC, ABCMeta
 from diot import Diot
 
-from .utils import cached_property
 from .pipen import Pipen
 from .proc import Proc
 
 
 class ProcGropuMeta(ABCMeta):
     """Meta class for ProcGroup"""
```

### Comparing `pipen-0.8.0/pipen/progressbar.py` & `pipen-0.9.0/pipen/progressbar.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/template.py` & `pipen-0.9.0/pipen/template.py`

 * *Files identical despite different names*

### Comparing `pipen-0.8.0/pipen/utils.py` & `pipen-0.9.0/pipen/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,25 +38,15 @@
     CONSOLE_WIDTH_SHIFT,
     LOGGER_NAME,
 )
 from .exceptions import ConfigurationError
 from .pluginmgr import plugin
 from .version import __version__
 
-try:  # pragma: no cover
-    from functools import cached_property
-except ImportError:  # pragma: no cover
-    # python 3.7
-    from cached_property import cached_property
-
-try:  # pragma: no cover
-    from importlib import metadata as importlib_metadata
-except ImportError:  # pragma: no cover
-    # python 3.7
-    import importlib_metadata
+from importlib import metadata as importlib_metadata
 
 if TYPE_CHECKING:  # pragma: no cover
     import pandas
     from rich.segment import Segment
     from rich.console import RenderableType
 
     from .proc import Proc
@@ -435,39 +425,45 @@
     return mtime
 
 
 def is_subclass(obj: Any, cls: type) -> bool:
     """Tell if obj is a subclass of cls
     Differences with issubclass is that we don't raise Type error if obj
     is not a class
+
     Args:
         obj: The object to check
         cls: The class to check
+
     Returns:
         True if obj is a subclass of cls otherwise False
     """
     try:
         return issubclass(obj, cls)
     except TypeError:
         return False
 
 
-def load_entrypoints(group: str) -> Iterable[Tuple[str, Any]]:
+def load_entrypoints(
+    group: str
+) -> Iterable[Tuple[str, Any]]:  # pragma: no cover
     """Load objects from setuptools entrypoints by given group name
+
     Args:
         group: The group name of the entrypoints
+
     Returns:
         An iterable of tuples with name and the loaded object
     """
-    for dist in importlib_metadata.distributions():  # pragma: no cover
-        for epoint in dist.entry_points:
-            if epoint.group != group:
-                continue
-            obj = epoint.load()
-            yield (epoint.name, obj)
+    try:
+        eps = importlib_metadata.entry_points(group=group)
+    except TypeError:
+        eps = importlib_metadata.entry_points().get(group, [])  # type: ignore
+
+    yield from ((ep.name, ep.load()) for ep in eps)
 
 
 def truncate_text(text: str, width: int, end: str = "…") -> str:
     """Truncate a text not based on words/whitespaces
     Otherwise, we could use textwrap.shorten.
 
     Args:
```

### Comparing `pipen-0.8.0/pyproject.toml` & `pipen-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "pipen"
-version = "0.8.0"
+version = "0.9.0"
 description = "A pipeline framework for python"
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen"
 repository = "https://github.com/pwwang/pipen"
 
@@ -16,32 +16,31 @@
 generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = "^3.8" # align with datar/pandas
 liquidpy = "^0.8"
 pandas = "^1.4"
 enlighten = "^1"
-cached-property = "^1"
 argx = "^0.2"
-xqute = "^0.1"
+xqute = "^0.2"
 ## included in xqute
 # rich = "^12"
 # diot = "^0.1"
 # simplug = "^0.0"
 ## including rtoml
 python-simpleconf = {version = "^0.5", extras = ["toml"]}
-pipda = "^0.11"
+pipda = "^0.12"
 varname = "^0.11"
 
 [tool.poetry.dev-dependencies]
 openpyxl = "^3"
 pytest = "^7"
 pytest-cov = "^4"
 pytest-xdist = "^3"
-datar = { version = "^0.11", extras = ["pandas"] }
+datar = { version = "^0.12", extras = ["pandas"] }
 
 [tool.poetry.scripts]
 pipen = "pipen.cli:main"
 
 [tool.pytest.ini_options]
 addopts = "-vv -n auto -p no:asyncio -p no:benchmark -W error::UserWarning --cov-config=.coveragerc --cov=pipen --cov-report xml:.coverage.xml --cov-report term-missing"
 # addopts = "-vv -n auto -p no:asyncio -W error::UserWarning"
```

### Comparing `pipen-0.8.0/setup.py` & `pipen-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,31 +5,30 @@
 ['pipen', 'pipen.cli']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['argx>=0.2,<0.3',
- 'cached-property>=1,<2',
  'enlighten>=1,<2',
  'liquidpy>=0.8,<0.9',
  'pandas>=1.4,<2.0',
- 'pipda>=0.11,<0.12',
+ 'pipda>=0.12,<0.13',
  'python-simpleconf[toml]>=0.5,<0.6',
  'varname>=0.11,<0.12',
- 'xqute>=0.1,<0.2']
+ 'xqute>=0.2,<0.3']
 
 entry_points = \
 {'console_scripts': ['pipen = pipen.cli:main']}
 
 setup_kwargs = {
     'name': 'pipen',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'A pipeline framework for python',
-    'long_description': '<div align="center">\n    <img src="./pipen.png" width="320px">\n\n**A pipeline framework for python**\n\n</div>\n\n______________________________________________________________________\n\n[![Pypi][6]][7] [![Github][8]][9] ![Building][10] [![Docs and API][11]][1] [![Codacy][12]][13] [![Codacy coverage][14]][13] [![Deps][5]][23]\n\n[Documentation][1] | [ChangeLog][2] | [Examples][3] | [API][4]\n\n## Features\n\n- Easy to use\n- Nearly zero-configuration\n- Nice logging\n- Highly extendable\n\n## Installation\n\n```bash\npip install -U pipen\n```\n\n## Quickstart\n\n`example.py`\n\n```python\nfrom pipen import Proc, Pipen\n\nclass P1(Proc):\n    """Sort input file"""\n    input = "infile"\n    input_data = ["/tmp/data.txt"]\n    output = "outfile:file:intermediate.txt"\n    script = "cat {{in.infile}} | sort > {{out.outfile}}"\n\nclass P2(Proc):\n    """Paste line number"""\n    requires = P1\n    input = "infile"\n    output = "outfile:file:result.txt"\n    script = "paste <(seq 1 3) {{in.infile}} > {{out.outfile}}"\n\nclass MyPipeline(Pipen):\n    starts = P1\n\nif __name__ == "__main__":\n    MyPipeline().run()\n```\n\n```shell\n> echo -e "3\\n2\\n1" > /tmp/data.txt\n> python example.py\n```\n\n```log\n[09/13/21 04:23:37] I main                    _____________________________________   __\n[09/13/21 04:23:37] I main                    ___  __ \\___  _/__  __ \\__  ____/__  | / /\n[09/13/21 04:23:37] I main                    __  /_/ /__  / __  /_/ /_  __/  __   |/ /\n[09/13/21 04:23:37] I main                    _  ____/__/ /  _  ____/_  /___  _  /|  /\n[09/13/21 04:23:37] I main                    /_/     /___/  /_/     /_____/  /_/ |_/\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main                                 version: 0.7.0\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭═════════════════════════════ MYPIPELIN ═══════════════════════════════╮\n[09/13/21 04:23:37] I main    ║  # procs          = 2                                                 ║\n[09/13/21 04:23:37] I main    ║  plugins          = [\'main\', \'verbose-0.0.1\']                         ║\n[09/13/21 04:23:37] I main    ║  profile          = default                                           ║\n[09/13/21 04:23:37] I main    ║  outdir           = mypipeline_results                                ║\n[09/13/21 04:23:37] I main    ║  cache            = True                                              ║\n[09/13/21 04:23:37] I main    ║  dirsig           = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  error_strategy   = ignore                                            ║\n[09/13/21 04:23:37] I main    ║  forks            = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  lang             = bash                                              ║\n[09/13/21 04:23:37] I main    ║  loglevel         = info                                              ║\n[09/13/21 04:23:37] I main    ║  num_retries      = 3                                                 ║\n[09/13/21 04:23:37] I main    ║  plugin_opts      = {}                                                ║\n[09/13/21 04:23:37] I main    ║  plugins          = None                                              ║\n[09/13/21 04:23:37] I main    ║  scheduler        = local                                             ║\n[09/13/21 04:23:37] I main    ║  scheduler_opts   = {}                                                ║\n[09/13/21 04:23:37] I main    ║  submission_batch = 8                                                 ║\n[09/13/21 04:23:37] I main    ║  template         = liquid                                            ║\n[09/13/21 04:23:37] I main    ║  template_opts    = {}                                                ║\n[09/13/21 04:23:37] I main    ║  workdir          = ./.pipen                                          ║\n[09/13/21 04:23:37] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭───────────────────────────────── P1 ──────────────────────────────────╮\n[09/13/21 04:23:37] I main    │ Sort input file                                                       │\n[09/13/21 04:23:37] I main    ╰───────────────────────────────────────────────────────────────────────╯\n[09/13/21 04:23:37] I main    P1: Workdir: \'.pipen/mypipeline/p1\'\n[09/13/21 04:23:37] I main    P1: <<< [START]\n[09/13/21 04:23:37] I main    P1: >>> [\'P2\']\n[09/13/21 04:23:37] I verbose P1: size: 1\n[09/13/21 04:23:37] I verbose P1: [0/0] in.infile: /tmp/data.txt\n[09/13/21 04:23:37] I verbose P1: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P1: Time elapsed: 00:00:01.039s\n[09/13/21 04:23:38] I main\n[09/13/21 04:23:38] I main    ╭═════════════════════════════════ P2 ══════════════════════════════════╮\n[09/13/21 04:23:38] I main    ║ Paste line number                                                     ║\n[09/13/21 04:23:38] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:38] I main    P2: Workdir: \'.pipen/mypipeline/p2\'\n[09/13/21 04:23:38] I main    P2: <<< [\'P1\']\n[09/13/21 04:23:38] I main    P2: >>> [END]\n[09/13/21 04:23:38] I verbose P2: size: 1\n[09/13/21 04:23:38] I verbose P2: [0/0] in.infile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P2: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/mypipeline_results/P2/result.txt\n[09/13/21 04:23:40] I verbose P2: Time elapsed: 00:00:02.074s\n[09/13/21 04:23:40] I main\n\n                PIPEN-0: 100%|████████████████████████████████████████| 2/2 [00:04<00:00, 0.56 procs/s]\n```\n\n```shell\n> cat ./mypipeline_results/P2/result.txt\n1       1\n2       2\n3       3\n```\n\n## Examples\n\nSee more examples at `examples/` and a more realcase example at:\nhttps://github.com/pwwang/pipen-report/tree/master/example\n\n## Plugin gallery\n\nPlugins make `pipen` even better.\n\n- [`pipen-verbose`][15]: Add verbosal information in logs for pipen.\n- [`pipen-lock`][25]: Process lock for pipen to prevent multiple runs at the same time.\n- [`pipen-report`][16]: Generate report for pipen\n- [`pipen-filters`][17]: Add a set of useful filters for pipen templates.\n- [`pipen-diagram`][18]: Draw pipeline diagrams for pipen\n- [`pipen-annotate`][26]: Use docstring to annotate pipen processes\n- [`pipen-args`][19]: Command line argument parser for pipen\n- [`pipen-dry`][20]: Dry runner for pipen pipelines\n- [`pipen-cli-init`][21]: A pipen CLI plugin to create a pipen project (pipeline)\n- [`pipen-cli-run`][22]: A pipen cli plugin to run a process or a pipeline\n- [`pipen-cli-config`][27]: UI wizard to generate configuration for pipen pipelines\n- [`pipen-cli-require`][24]: A pipen cli plugin check the requirements of a pipeline\n\n\n[1]: https://pwwang.github.io/pipen\n[2]: https://pwwang.github.io/pipen/CHANGELOG\n[3]: https://pwwang.github.io/pipen/examples\n[4]: https://pwwang.github.io/pipen/api/pipen\n[5]: https://img.shields.io/librariesio/release/pypi/pipen?style=flat-square\n[6]: https://img.shields.io/pypi/v/pipen?style=flat-square\n[7]: https://pypi.org/project/pipen/\n[8]: https://img.shields.io/github/v/tag/pwwang/pipen?style=flat-square\n[9]: https://github.com/pwwang/pipen\n[10]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/build.yml?style=flat-square\n[11]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/docs.yml?label=docs&style=flat-square\n[12]: https://img.shields.io/codacy/grade/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[13]: https://app.codacy.com/gh/pwwang/pipen\n[14]: https://img.shields.io/codacy/coverage/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[15]: https://github.com/pwwang/pipen-verbose\n[16]: https://github.com/pwwang/pipen-report\n[17]: https://github.com/pwwang/pipen-filters\n[18]: https://github.com/pwwang/pipen-diagram\n[19]: https://github.com/pwwang/pipen-args\n[20]: https://github.com/pwwang/pipen-dry\n[21]: https://github.com/pwwang/pipen-cli-init\n[22]: https://github.com/pwwang/pipen-cli-run\n[23]: https://libraries.io/github/pwwang/pipen#repository_dependencies\n[24]: https://github.com/pwwang/pipen-cli-require\n[25]: https://github.com/pwwang/pipen-lock\n[26]: https://github.com/pwwang/pipen-annotate\n[27]: https://github.com/pwwang/pipen-cli-config\n',
+    'long_description': '<div align="center">\n    <img src="./pipen.png" width="320px">\n\n**A pipeline framework for python**\n\n</div>\n\n______________________________________________________________________\n\n[![Pypi][6]][7] [![Github][8]][9] ![Building][10] [![Docs and API][11]][1] [![Codacy][12]][13] [![Codacy coverage][14]][13] [![Deps][5]][23]\n\n[Documentation][1] | [ChangeLog][2] | [Examples][3] | [API][4]\n\n## Features\n\n- Easy to use\n- Nearly zero-configuration\n- Nice logging\n- Highly extendable\n\n## Installation\n\n```bash\npip install -U pipen\n```\n\n## Quickstart\n\n`example.py`\n\n```python\nfrom pipen import Proc, Pipen\n\nclass P1(Proc):\n    """Sort input file"""\n    input = "infile"\n    input_data = ["/tmp/data.txt"]\n    output = "outfile:file:intermediate.txt"\n    script = "cat {{in.infile}} | sort > {{out.outfile}}"\n\nclass P2(Proc):\n    """Paste line number"""\n    requires = P1\n    input = "infile"\n    output = "outfile:file:result.txt"\n    script = "paste <(seq 1 3) {{in.infile}} > {{out.outfile}}"\n\nclass MyPipeline(Pipen):\n    starts = P1\n\nif __name__ == "__main__":\n    MyPipeline().run()\n```\n\n```shell\n> echo -e "3\\n2\\n1" > /tmp/data.txt\n> python example.py\n```\n\n```log\n[09/13/21 04:23:37] I main                    _____________________________________   __\n[09/13/21 04:23:37] I main                    ___  __ \\___  _/__  __ \\__  ____/__  | / /\n[09/13/21 04:23:37] I main                    __  /_/ /__  / __  /_/ /_  __/  __   |/ /\n[09/13/21 04:23:37] I main                    _  ____/__/ /  _  ____/_  /___  _  /|  /\n[09/13/21 04:23:37] I main                    /_/     /___/  /_/     /_____/  /_/ |_/\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main                                 version: 0.9.0\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭═════════════════════════════ MYPIPELIN ═══════════════════════════════╮\n[09/13/21 04:23:37] I main    ║  # procs          = 2                                                 ║\n[09/13/21 04:23:37] I main    ║  plugins          = [\'main\', \'verbose-0.0.1\']                         ║\n[09/13/21 04:23:37] I main    ║  profile          = default                                           ║\n[09/13/21 04:23:37] I main    ║  outdir           = mypipeline_results                                ║\n[09/13/21 04:23:37] I main    ║  cache            = True                                              ║\n[09/13/21 04:23:37] I main    ║  dirsig           = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  error_strategy   = ignore                                            ║\n[09/13/21 04:23:37] I main    ║  forks            = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  lang             = bash                                              ║\n[09/13/21 04:23:37] I main    ║  loglevel         = info                                              ║\n[09/13/21 04:23:37] I main    ║  num_retries      = 3                                                 ║\n[09/13/21 04:23:37] I main    ║  plugin_opts      = {}                                                ║\n[09/13/21 04:23:37] I main    ║  plugins          = None                                              ║\n[09/13/21 04:23:37] I main    ║  scheduler        = local                                             ║\n[09/13/21 04:23:37] I main    ║  scheduler_opts   = {}                                                ║\n[09/13/21 04:23:37] I main    ║  submission_batch = 8                                                 ║\n[09/13/21 04:23:37] I main    ║  template         = liquid                                            ║\n[09/13/21 04:23:37] I main    ║  template_opts    = {}                                                ║\n[09/13/21 04:23:37] I main    ║  workdir          = ./.pipen                                          ║\n[09/13/21 04:23:37] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭───────────────────────────────── P1 ──────────────────────────────────╮\n[09/13/21 04:23:37] I main    │ Sort input file                                                       │\n[09/13/21 04:23:37] I main    ╰───────────────────────────────────────────────────────────────────────╯\n[09/13/21 04:23:37] I main    P1: Workdir: \'.pipen/mypipeline/p1\'\n[09/13/21 04:23:37] I main    P1: <<< [START]\n[09/13/21 04:23:37] I main    P1: >>> [\'P2\']\n[09/13/21 04:23:37] I verbose P1: size: 1\n[09/13/21 04:23:37] I verbose P1: [0/0] in.infile: /tmp/data.txt\n[09/13/21 04:23:37] I verbose P1: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P1: Time elapsed: 00:00:01.039s\n[09/13/21 04:23:38] I main\n[09/13/21 04:23:38] I main    ╭═════════════════════════════════ P2 ══════════════════════════════════╮\n[09/13/21 04:23:38] I main    ║ Paste line number                                                     ║\n[09/13/21 04:23:38] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:38] I main    P2: Workdir: \'.pipen/mypipeline/p2\'\n[09/13/21 04:23:38] I main    P2: <<< [\'P1\']\n[09/13/21 04:23:38] I main    P2: >>> [END]\n[09/13/21 04:23:38] I verbose P2: size: 1\n[09/13/21 04:23:38] I verbose P2: [0/0] in.infile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P2: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/mypipeline_results/P2/result.txt\n[09/13/21 04:23:40] I verbose P2: Time elapsed: 00:00:02.074s\n[09/13/21 04:23:40] I main\n\n                PIPEN-0: 100%|████████████████████████████████████████| 2/2 [00:04<00:00, 0.56 procs/s]\n```\n\n```shell\n> cat ./mypipeline_results/P2/result.txt\n1       1\n2       2\n3       3\n```\n\n## Examples\n\nSee more examples at `examples/` and a more realcase example at:\nhttps://github.com/pwwang/pipen-report/tree/master/example\n\n## Plugin gallery\n\nPlugins make `pipen` even better.\n\n- [`pipen-verbose`][15]: Add verbosal information in logs for pipen.\n- [`pipen-lock`][25]: Process lock for pipen to prevent multiple runs at the same time.\n- [`pipen-report`][16]: Generate report for pipen\n- [`pipen-filters`][17]: Add a set of useful filters for pipen templates.\n- [`pipen-diagram`][18]: Draw pipeline diagrams for pipen\n- [`pipen-annotate`][26]: Use docstring to annotate pipen processes\n- [`pipen-args`][19]: Command line argument parser for pipen\n- [`pipen-dry`][20]: Dry runner for pipen pipelines\n- [`pipen-cli-init`][21]: A pipen CLI plugin to create a pipen project (pipeline)\n- [`pipen-cli-run`][22]: A pipen cli plugin to run a process or a pipeline\n- [`pipen-cli-config`][27]: UI wizard to generate configuration for pipen pipelines\n- [`pipen-cli-require`][24]: A pipen cli plugin check the requirements of a pipeline\n\n\n[1]: https://pwwang.github.io/pipen\n[2]: https://pwwang.github.io/pipen/CHANGELOG\n[3]: https://pwwang.github.io/pipen/examples\n[4]: https://pwwang.github.io/pipen/api/pipen\n[5]: https://img.shields.io/librariesio/release/pypi/pipen?style=flat-square\n[6]: https://img.shields.io/pypi/v/pipen?style=flat-square\n[7]: https://pypi.org/project/pipen/\n[8]: https://img.shields.io/github/v/tag/pwwang/pipen?style=flat-square\n[9]: https://github.com/pwwang/pipen\n[10]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/build.yml?style=flat-square\n[11]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/docs.yml?label=docs&style=flat-square\n[12]: https://img.shields.io/codacy/grade/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[13]: https://app.codacy.com/gh/pwwang/pipen\n[14]: https://img.shields.io/codacy/coverage/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[15]: https://github.com/pwwang/pipen-verbose\n[16]: https://github.com/pwwang/pipen-report\n[17]: https://github.com/pwwang/pipen-filters\n[18]: https://github.com/pwwang/pipen-diagram\n[19]: https://github.com/pwwang/pipen-args\n[20]: https://github.com/pwwang/pipen-dry\n[21]: https://github.com/pwwang/pipen-cli-init\n[22]: https://github.com/pwwang/pipen-cli-run\n[23]: https://libraries.io/github/pwwang/pipen#repository_dependencies\n[24]: https://github.com/pwwang/pipen-cli-require\n[25]: https://github.com/pwwang/pipen-lock\n[26]: https://github.com/pwwang/pipen-annotate\n[27]: https://github.com/pwwang/pipen-cli-config\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pipen-0.8.0/PKG-INFO` & `pipen-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pipen
-Version: 0.8.0
+Version: 0.9.0
 Summary: A pipeline framework for python
 Home-page: https://github.com/pwwang/pipen
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argx (>=0.2,<0.3)
-Requires-Dist: cached-property (>=1,<2)
 Requires-Dist: enlighten (>=1,<2)
 Requires-Dist: liquidpy (>=0.8,<0.9)
 Requires-Dist: pandas (>=1.4,<2.0)
-Requires-Dist: pipda (>=0.11,<0.12)
+Requires-Dist: pipda (>=0.12,<0.13)
 Requires-Dist: python-simpleconf[toml] (>=0.5,<0.6)
 Requires-Dist: varname (>=0.11,<0.12)
-Requires-Dist: xqute (>=0.1,<0.2)
+Requires-Dist: xqute (>=0.2,<0.3)
 Project-URL: Repository, https://github.com/pwwang/pipen
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="./pipen.png" width="320px">
 
 **A pipeline framework for python**
@@ -87,15 +86,15 @@
 ```log
 [09/13/21 04:23:37] I main                    _____________________________________   __
 [09/13/21 04:23:37] I main                    ___  __ \___  _/__  __ \__  ____/__  | / /
 [09/13/21 04:23:37] I main                    __  /_/ /__  / __  /_/ /_  __/  __   |/ /
 [09/13/21 04:23:37] I main                    _  ____/__/ /  _  ____/_  /___  _  /|  /
 [09/13/21 04:23:37] I main                    /_/     /___/  /_/     /_____/  /_/ |_/
 [09/13/21 04:23:37] I main
-[09/13/21 04:23:37] I main                                 version: 0.7.0
+[09/13/21 04:23:37] I main                                 version: 0.9.0
 [09/13/21 04:23:37] I main
 [09/13/21 04:23:37] I main    ╭═════════════════════════════ MYPIPELIN ═══════════════════════════════╮
 [09/13/21 04:23:37] I main    ║  # procs          = 2                                                 ║
 [09/13/21 04:23:37] I main    ║  plugins          = ['main', 'verbose-0.0.1']                         ║
 [09/13/21 04:23:37] I main    ║  profile          = default                                           ║
 [09/13/21 04:23:37] I main    ║  outdir           = mypipeline_results                                ║
 [09/13/21 04:23:37] I main    ║  cache            = True                                              ║
```

