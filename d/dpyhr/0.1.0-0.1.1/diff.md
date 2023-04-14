# Comparing `tmp/dpyhr-0.1.0.tar.gz` & `tmp/dpyhr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpyhr-0.1.0.tar", max compression
+gzip compressed data, was "dpyhr-0.1.1.tar", max compression
```

## Comparing `dpyhr-0.1.0.tar` & `dpyhr-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1076 2023-01-17 15:23:02.035930 dpyhr-0.1.0/LICENSE
--rw-r--r--   0        0        0     1311 2023-01-17 15:23:02.035930 dpyhr-0.1.0/README.md
--rw-r--r--   0        0        0     1601 2023-01-17 15:23:02.039930 dpyhr-0.1.0/dpyhr/__init__.py
--rw-r--r--   0        0        0     1492 2023-01-17 15:23:02.039930 dpyhr-0.1.0/dpyhr/normal.py
--rw-r--r--   0        0        0     1529 2023-01-17 15:23:02.039930 dpyhr-0.1.0/dpyhr/polling.py
--rw-r--r--   0        0        0      641 2023-01-17 15:23:02.039930 dpyhr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2028 1970-01-01 00:00:00.000000 dpyhr-0.1.0/setup.py
--rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 dpyhr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-14 06:09:29.692891 dpyhr-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1757 2023-04-14 06:09:29.692891 dpyhr-0.1.1/README.md
+-rw-r--r--   0        0        0     3380 2023-04-14 06:09:29.692891 dpyhr-0.1.1/dpyhr/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-14 06:09:29.692891 dpyhr-0.1.1/dpyhr/log_dummy.py
+-rw-r--r--   0        0        0     1844 2023-04-14 06:09:29.692891 dpyhr-0.1.1/dpyhr/normal.py
+-rw-r--r--   0        0        0     1899 2023-04-14 06:09:29.692891 dpyhr-0.1.1/dpyhr/polling.py
+-rw-r--r--   0        0        0     1158 2023-04-14 06:09:29.692891 dpyhr-0.1.1/dpyhr/utils.py
+-rw-r--r--   0        0        0      662 2023-04-14 06:09:29.692891 dpyhr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 dpyhr-0.1.1/PKG-INFO
```

### Comparing `dpyhr-0.1.0/LICENSE` & `dpyhr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dpyhr-0.1.0/README.md` & `dpyhr-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,27 +5,40 @@
 
 1. Install dpyhr with pip (`pip install dpyhr`)
 2. Import dpyhr and run it with
 
 ```py
 import dpyhr
 
-dpyhr.run(bot: commands.Bot, *paths: str, selection: Selection = Selection.normal, reloader: typing.Callable=None, conditional: typing.Callable=None, recursive: bool=False, **kwargs)
+dpyhr.run(
+    *paths: str,
+    bot: commands.Bot = None,
+    selection: Selection = Selection.normal,
+    reloader: typing.Callable = None,
+    conditional: typing.Callable = None,
+    recursive: bool = False,
+    **kwargs
+)
 ```
 
 `dpyhr.run` have a documentation as this
 
-> Run dphyr in another thread.
+> Run dphyr in another thread.  
 
->   Args:
->        bot (commands.Bot): For reloading extensions (if reloader doesn't exists)
->        selection (Selection, optional): Observer selection. Defaults to Selection.normal.
->        reloader (typing.Callable, optional): Reload module with your own function. Defaults to None.
->        conditional (typing.Callable, optional): Conditional when event is triggered. Defaults to None.
->       recursive (bool, optional): Recursive reloading. Defaults to False.
->        **kwargs: Other arguments for observer.
->    Returns:
->        None: No returns.
+>    Args:  
+>        *paths (str): Paths you want to watch for cogs. Supply those as argument  
+>        bot (commands.Bot, Optional): For reloading extensions (if reloader doesn't exists)  
+>        selection (Selection, optional): Observer selection. Defaults to Selection.normal.  
+>        reloader (typing.Callable, optional): Reload module with your own function. Defaults to None.  
+>        conditional (typing.Callable, optional): Conditional when event is triggered. Defaults to None.  
+>        recursive (bool, optional): Recursive reloading. Defaults to False.  
+>        **kwargs: Other arguments for observer.  
+>    Returns:  
+>        None: No returns.  
 
 ## Caution
 
 dpyhr wouldn't work if you called your bot outside of the entrypoint starter so nested path wouldn't work in this case. you need to run it inside directory where you want python file to run else reloader might get wrong path and spits errors out.
+
+## Why you don't shipped discord.py with this package?
+
+Because dpyhr is trying to be able to compatible with any discord.py versions that have `discord.ext.commands` (other discord.py forks should works if they have `commands.Bot.reload_extension` and their package name is `discord`)
```

### Comparing `dpyhr-0.1.0/dpyhr/polling.py` & `dpyhr-0.1.1/dpyhr/normal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,65 @@
-from watchdog.events import FileSystemEventHandler, FileSystemEvent
-from watchdog.observers.polling import PollingObserver as Observer
-import asyncio
-import logging
 import traceback
 import typing
 
-log = logging.getLogger("dphyr.polling")
+from watchdog.events import FileSystemEvent, FileSystemEventHandler
+from watchdog.observers import Observer
 
-class Polling(FileSystemEventHandler):
+from .log_dummy import Logger
+from .utils import prevent_calling_outside_dpyhr, runner
+
+log = Logger("dpyhr.normal")
+
+
+class Normal(FileSystemEventHandler):
     def __init__(self, reloader: typing.Callable, condition: typing.Callable) -> None:
         self.reload = reloader
         self.condition = condition
+
     def on_modified(self, event: FileSystemEvent) -> typing.NoReturn:
         log.info(f"File changed: {event.src_path}")
-        if self.condition(event):
+        if runner(self.condition, event):
             log.info("Reloading...")
-            path = event.src_path.replace("\\", "/").replace("/", ".")[:-3] # Convert to module path :D
+            path = event.src_path.replace("\\", "/").replace("/", ".")[
+                :-3
+            ]  # Convert to module path :D
             try:
-                asyncio.run(self.reload(path))
+                runner(self.reload, path)
                 log.info(f"Reloaded {path}")
             except Exception as e:
                 log.error(f"Failed to reload {path}")
                 log.error(e)
                 log.error(traceback.format_exc())
-                
-def polling_start(*paths: str, reloader: typing.Callable, condition: typing.Callable, recursive: bool, **kwargs) -> typing.NoReturn:
+
+
+@prevent_calling_outside_dpyhr
+def enable_log():
+    global log
+    import logging
+
+    log = logging.getLogger("dpyhr.normal")
+
+
+@prevent_calling_outside_dpyhr
+def disable_log():
+    global log
+    log = Logger("dpyhr.normal")
+
+
+@prevent_calling_outside_dpyhr
+def start(
+    *paths: str,
+    reloader: typing.Callable,
+    condition: typing.Callable,
+    recursive: bool,
+    **kwargs,
+) -> typing.NoReturn:
     """
     Internal function for starting normal observer.
     Please use dphyr.run() instead.
     """
     normal_observer = Observer(**kwargs)
     for path in paths:
         log.debug(f"Adding {path} to observer")
-        normal_observer.schedule(Polling(reloader, condition), path, recursive=recursive)
+        normal_observer.schedule(Normal(reloader, condition), path, recursive=recursive)
     normal_observer.start()
-    log.info("Started polling observer")
+    log.info("Started normal observer")
```

### Comparing `dpyhr-0.1.0/pyproject.toml` & `dpyhr-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "dpyhr"
-version = "0.1.0"
+version = "0.1.1"
 description = "dpyhr. A discord.py module reloader written in pure python!"
 authors = ["timelessnesses <mooping3roblox@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/timelessnesses/dpyhr"
 repository = "https://github.com/timelessnesses/dpyhr"
 packages = [
     { include = "./dpyhr" },
 ]
 [tool.poetry.dependencies]
 python = "^3.8"
 watchdog = "^2.2.1"
+decohints = "^1.0.7"
 
 [tool.poetry.group.dev.dependencies]
 "discord.py" = "^2.1.0"
 black = "^22.12.0"
 isort = "^5.11.4"
 python-dotenv = "^0.21.0"
```

### Comparing `dpyhr-0.1.0/setup.py` & `dpyhr-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,65 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dpyhr
+Version: 0.1.1
+Summary: dpyhr. A discord.py module reloader written in pure python!
+Home-page: https://github.com/timelessnesses/dpyhr
+License: MIT
+Author: timelessnesses
+Author-email: mooping3roblox@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: decohints (>=1.0.7,<2.0.0)
+Requires-Dist: watchdog (>=2.2.1,<3.0.0)
+Project-URL: Repository, https://github.com/timelessnesses/dpyhr
+Description-Content-Type: text/markdown
+
+# dpyhr
+dpyhr is a hot cog reloader (that uses discord.py cog's implementation) to reload anytime you wanted to save!
+
+## Setup
+
+1. Install dpyhr with pip (`pip install dpyhr`)
+2. Import dpyhr and run it with
+
+```py
+import dpyhr
+
+dpyhr.run(
+    *paths: str,
+    bot: commands.Bot = None,
+    selection: Selection = Selection.normal,
+    reloader: typing.Callable = None,
+    conditional: typing.Callable = None,
+    recursive: bool = False,
+    **kwargs
+)
+```
+
+`dpyhr.run` have a documentation as this
+
+> Run dphyr in another thread.  
+
+>    Args:  
+>        *paths (str): Paths you want to watch for cogs. Supply those as argument  
+>        bot (commands.Bot, Optional): For reloading extensions (if reloader doesn't exists)  
+>        selection (Selection, optional): Observer selection. Defaults to Selection.normal.  
+>        reloader (typing.Callable, optional): Reload module with your own function. Defaults to None.  
+>        conditional (typing.Callable, optional): Conditional when event is triggered. Defaults to None.  
+>        recursive (bool, optional): Recursive reloading. Defaults to False.  
+>        **kwargs: Other arguments for observer.  
+>    Returns:  
+>        None: No returns.  
 
-packages = \
-['dpyhr']
+## Caution
 
-package_data = \
-{'': ['*']}
+dpyhr wouldn't work if you called your bot outside of the entrypoint starter so nested path wouldn't work in this case. you need to run it inside directory where you want python file to run else reloader might get wrong path and spits errors out.
 
-install_requires = \
-['watchdog>=2.2.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'dpyhr',
-    'version': '0.1.0',
-    'description': 'dpyhr. A discord.py module reloader written in pure python!',
-    'long_description': "# dpyhr\ndpyhr is a hot cog reloader (that uses discord.py cog's implementation) to reload anytime you wanted to save!\n\n## Setup\n\n1. Install dpyhr with pip (`pip install dpyhr`)\n2. Import dpyhr and run it with\n\n```py\nimport dpyhr\n\ndpyhr.run(bot: commands.Bot, *paths: str, selection: Selection = Selection.normal, reloader: typing.Callable=None, conditional: typing.Callable=None, recursive: bool=False, **kwargs)\n```\n\n`dpyhr.run` have a documentation as this\n\n> Run dphyr in another thread.\n\n>   Args:\n>        bot (commands.Bot): For reloading extensions (if reloader doesn't exists)\n>        selection (Selection, optional): Observer selection. Defaults to Selection.normal.\n>        reloader (typing.Callable, optional): Reload module with your own function. Defaults to None.\n>        conditional (typing.Callable, optional): Conditional when event is triggered. Defaults to None.\n>       recursive (bool, optional): Recursive reloading. Defaults to False.\n>        **kwargs: Other arguments for observer.\n>    Returns:\n>        None: No returns.\n\n## Caution\n\ndpyhr wouldn't work if you called your bot outside of the entrypoint starter so nested path wouldn't work in this case. you need to run it inside directory where you want python file to run else reloader might get wrong path and spits errors out.\n",
-    'author': 'timelessnesses',
-    'author_email': 'mooping3roblox@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/timelessnesses/dpyhr',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+## Why you don't shipped discord.py with this package?
 
+Because dpyhr is trying to be able to compatible with any discord.py versions that have `discord.ext.commands` (other discord.py forks should works if they have `commands.Bot.reload_extension` and their package name is `discord`)
 
-setup(**setup_kwargs)
```

