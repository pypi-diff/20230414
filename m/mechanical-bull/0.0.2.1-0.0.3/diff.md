# Comparing `tmp/mechanical_bull-0.0.2.1.tar.gz` & `tmp/mechanical_bull-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanical_bull-0.0.2.1.tar", max compression
+gzip compressed data, was "mechanical_bull-0.0.3.tar", max compression
```

## Comparing `mechanical_bull-0.0.2.1.tar` & `mechanical_bull-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1062 2023-03-24 18:08:48.112283 mechanical_bull-0.0.2.1/LICENSE
--rw-r--r--   0        0        0     1797 2023-04-14 13:55:07.334603 mechanical_bull-0.0.2.1/README.md
--rw-r--r--   0        0        0      439 2023-04-14 10:56:36.800916 mechanical_bull-0.0.2.1/mechanical_bull/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:57:25.358266 mechanical_bull-0.0.2.1/mechanical_bull/actions/__init__.py
--rw-r--r--   0        0        0      465 2023-04-14 12:53:46.015259 mechanical_bull-0.0.2.1/mechanical_bull/actions/handle_follow_request.py
--rw-r--r--   0        0        0      225 2023-04-14 13:32:31.198189 mechanical_bull-0.0.2.1/mechanical_bull/actions/log_to_file.py
--rw-r--r--   0        0        0      600 2023-04-14 12:54:03.319364 mechanical_bull-0.0.2.1/mechanical_bull/actions/test_handle_follow_request.py
--rw-r--r--   0        0        0     1357 2023-04-14 13:38:28.993309 mechanical_bull-0.0.2.1/mechanical_bull/add_user.py
--rw-r--r--   0        0        0      385 2023-04-14 10:25:27.028750 mechanical_bull-0.0.2.1/mechanical_bull/event_loop.py
--rw-r--r--   0        0        0      335 2023-04-14 13:31:35.265702 mechanical_bull-0.0.2.1/mechanical_bull/handlers.py
--rw-r--r--   0        0        0      517 2023-04-14 13:41:44.931018 mechanical_bull-0.0.2.1/mechanical_bull/run.py
--rw-r--r--   0        0        0      556 2023-04-14 10:25:41.080898 mechanical_bull-0.0.2.1/mechanical_bull/test_event_loop.py
--rw-r--r--   0        0        0      484 2023-04-14 13:32:17.358069 mechanical_bull-0.0.2.1/mechanical_bull/test_handlers.py
--rw-r--r--   0        0        0      708 2023-04-14 13:56:13.268348 mechanical_bull-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 mechanical_bull-0.0.2.1/setup.py
--rw-r--r--   0        0        0     2414 1970-01-01 00:00:00.000000 mechanical_bull-0.0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-03-24 18:08:48.112283 mechanical_bull-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1798 2023-04-14 13:57:27.250172 mechanical_bull-0.0.3/README.md
+-rw-r--r--   0        0        0      439 2023-04-14 10:56:36.800916 mechanical_bull-0.0.3/mechanical_bull/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:57:25.358266 mechanical_bull-0.0.3/mechanical_bull/actions/__init__.py
+-rw-r--r--   0        0        0      491 2023-04-14 14:07:32.437682 mechanical_bull-0.0.3/mechanical_bull/actions/handle_follow_request.py
+-rw-r--r--   0        0        0      225 2023-04-14 13:32:31.198189 mechanical_bull-0.0.3/mechanical_bull/actions/log_to_file.py
+-rw-r--r--   0        0        0      600 2023-04-14 12:54:03.319364 mechanical_bull-0.0.3/mechanical_bull/actions/test_handle_follow_request.py
+-rw-r--r--   0        0        0     1357 2023-04-14 13:38:28.993309 mechanical_bull-0.0.3/mechanical_bull/add_user.py
+-rw-r--r--   0        0        0      480 2023-04-14 14:07:14.953405 mechanical_bull-0.0.3/mechanical_bull/event_loop.py
+-rw-r--r--   0        0        0      335 2023-04-14 13:31:35.265702 mechanical_bull-0.0.3/mechanical_bull/handlers.py
+-rw-r--r--   0        0        0      637 2023-04-14 14:25:25.580435 mechanical_bull-0.0.3/mechanical_bull/run.py
+-rw-r--r--   0        0        0      556 2023-04-14 10:25:41.080898 mechanical_bull-0.0.3/mechanical_bull/test_event_loop.py
+-rw-r--r--   0        0        0      484 2023-04-14 13:32:17.358069 mechanical_bull-0.0.3/mechanical_bull/test_handlers.py
+-rw-r--r--   0        0        0      706 2023-04-14 14:25:48.460725 mechanical_bull-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 mechanical_bull-0.0.3/setup.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 mechanical_bull-0.0.3/PKG-INFO
```

### Comparing `mechanical_bull-0.0.2.1/LICENSE` & `mechanical_bull-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.2.1/README.md` & `mechanical_bull-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,9 +35,9 @@
     return
 ```
 
 here the kwargs are the dict given by the definiton in the handler block, i.e.
 
 ```toml
 [user.handlers]
-"my.package": { arg1 = "value1", arg2 = "value2 }
+"my.package" = { arg1 = "value1", arg2 = "value2 }
 ```
```

### Comparing `mechanical_bull-0.0.2.1/mechanical_bull/actions/test_handle_follow_request.py` & `mechanical_bull-0.0.3/mechanical_bull/actions/test_handle_follow_request.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.2.1/mechanical_bull/add_user.py` & `mechanical_bull-0.0.3/mechanical_bull/add_user.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.2.1/mechanical_bull/run.py` & `mechanical_bull-0.0.3/mechanical_bull/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import tomllib
 import asyncio
+import logging
 
 from .event_loop import loop
 from .handlers import load_handlers
 
 
 async def mechanical_bull(config_file):
     with open(config_file, "rb") as fp:
         config = tomllib.load(fp)
 
+    if "logfile" in config:
+        logging.basicConfig(level=logging.INFO, filename=config["logfile"])
+
     async with asyncio.TaskGroup() as taskgroup:
         for _, value in config.items():
             handlers = load_handlers(value["handlers"])
             taskgroup.create_task(loop(value, handlers))
 
 
 def main():
```

### Comparing `mechanical_bull-0.0.2.1/mechanical_bull/test_event_loop.py` & `mechanical_bull-0.0.3/mechanical_bull/test_event_loop.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.2.1/pyproject.toml` & `mechanical_bull-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mechanical-bull"
-version = "0.0.2.1"
+version = "0.0.3"
 description = "A framework to automate reacting to ActivityStreams events."
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "mechanical_bull"}]
 repository = "https://codeberg.org/helge/mechanical_bull"
```

### Comparing `mechanical_bull-0.0.2.1/setup.py` & `mechanical_bull-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['bovine>=0.1.0,<0.2.0', 'tomli-w>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'mechanical-bull',
-    'version': '0.0.2.1',
+    'version': '0.0.3',
     'description': 'A framework to automate reacting to ActivityStreams events.',
-    'long_description': '# Mechanical Bull\n\nMechanical Bull is an ActivityPub Client application build based on [bovine](https://codeberg.org/helge/bovine/). It\'s main goal is to provide a platform for automating activities undertaking in the FediVerse. Furthermore, it serves as a demonstration how ActivityPub Clients can be build with bovine.\n\n## Installation\n\nOne can simply install mechanical_bull with pip via\n\n```bash\npip install mechanical-bull\n```\n\nOnce can then add a new user by running\n\n```bash\npython -m mechanical_bull.add_user\n```\n\nThis will then ask you to enter a name, the hostname, your ActivityPub Actor lives on, then prompt you to add a new did:key to your ActivityPub Actor. This did:key will be used to authenticate mechanical_bull against your server. Once you have added the key, press enter, and mechanical_bull is running. This method of authentication is called Moo-Auth-1 and described [here](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation).\n\nThe configuration is saved in `config.toml`. bovine also supports authentication through private keys and HTTP signatures. For the details on how to configure this, please consult bovine. You can add further automations there.\n\nThen you should be able to run mechanical bull via\n\n```bash\npython -m mechanical_bull.run\n```\n\n## Writing automations\n\nThe examples of `mechanical_bull.actions.handle_follow_request` and `mechanical_bull.actions.log_to_file` should show how to write a new automation. The basic idea is that each file contains a function handle with signature\n\n```python\nasync def handle(client: BovineClient, data: dict, **kwargs):\n    return\n```\n\nhere the kwargs are the dict given by the definiton in the handler block, i.e.\n\n```toml\n[user.handlers]\n"my.package": { arg1 = "value1", arg2 = "value2 }\n```\n',
+    'long_description': '# Mechanical Bull\n\nMechanical Bull is an ActivityPub Client application build based on [bovine](https://codeberg.org/helge/bovine/). It\'s main goal is to provide a platform for automating activities undertaking in the FediVerse. Furthermore, it serves as a demonstration how ActivityPub Clients can be build with bovine.\n\n## Installation\n\nOne can simply install mechanical_bull with pip via\n\n```bash\npip install mechanical-bull\n```\n\nOnce can then add a new user by running\n\n```bash\npython -m mechanical_bull.add_user\n```\n\nThis will then ask you to enter a name, the hostname, your ActivityPub Actor lives on, then prompt you to add a new did:key to your ActivityPub Actor. This did:key will be used to authenticate mechanical_bull against your server. Once you have added the key, press enter, and mechanical_bull is running. This method of authentication is called Moo-Auth-1 and described [here](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation).\n\nThe configuration is saved in `config.toml`. bovine also supports authentication through private keys and HTTP signatures. For the details on how to configure this, please consult bovine. You can add further automations there.\n\nThen you should be able to run mechanical bull via\n\n```bash\npython -m mechanical_bull.run\n```\n\n## Writing automations\n\nThe examples of `mechanical_bull.actions.handle_follow_request` and `mechanical_bull.actions.log_to_file` should show how to write a new automation. The basic idea is that each file contains a function handle with signature\n\n```python\nasync def handle(client: BovineClient, data: dict, **kwargs):\n    return\n```\n\nhere the kwargs are the dict given by the definiton in the handler block, i.e.\n\n```toml\n[user.handlers]\n"my.package" = { arg1 = "value1", arg2 = "value2 }\n```\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/helge/mechanical_bull',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mechanical_bull-0.0.2.1/PKG-INFO` & `mechanical_bull-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanical-bull
-Version: 0.0.2.1
+Version: 0.0.3
 Summary: A framework to automate reacting to ActivityStreams events.
 Home-page: https://codeberg.org/helge/mechanical_bull
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -52,10 +52,10 @@
     return
 ```
 
 here the kwargs are the dict given by the definiton in the handler block, i.e.
 
 ```toml
 [user.handlers]
-"my.package": { arg1 = "value1", arg2 = "value2 }
+"my.package" = { arg1 = "value1", arg2 = "value2 }
 ```
```

