# Comparing `tmp/connpy-2.1.8.tar.gz` & `tmp/connpy-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-2.1.8.tar", last modified: Tue Mar 21 21:26:10 2023, max compression
+gzip compressed data, was "connpy-3.0.0.tar", last modified: Fri Apr 14 14:48:54 2023, max compression
```

## Comparing `connpy-2.1.8.tar` & `connpy-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:26:10.593824 connpy-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-21 21:25:57.000000 connpy-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-03-21 21:26:10.593824 connpy-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-03-21 21:25:57.000000 connpy-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:26:10.589824 connpy-2.1.8/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-03-21 21:25:57.000000 connpy-2.1.8/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-21 21:25:57.000000 connpy-2.1.8/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-21 21:25:57.000000 connpy-2.1.8/connpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-21 21:25:57.000000 connpy-2.1.8/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9047 2023-03-21 21:25:57.000000 connpy-2.1.8/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48186 2023-03-21 21:25:57.000000 connpy-2.1.8/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27912 2023-03-21 21:25:57.000000 connpy-2.1.8/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:26:10.589824 connpy-2.1.8/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-03-21 21:26:10.000000 connpy-2.1.8/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-21 21:26:10.000000 connpy-2.1.8/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 21:26:10.000000 connpy-2.1.8/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-21 21:26:10.000000 connpy-2.1.8/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-21 21:26:10.000000 connpy-2.1.8/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-21 21:26:10.000000 connpy-2.1.8/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-21 21:26:10.593824 connpy-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-21 21:25:57.000000 connpy-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:48:54.647227 connpy-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 14:48:44.000000 connpy-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 14:48:54.647227 connpy-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-14 14:48:44.000000 connpy-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:48:54.647227 connpy-3.0.0/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-14 14:48:44.000000 connpy-3.0.0/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 14:48:44.000000 connpy-3.0.0/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 14:48:44.000000 connpy-3.0.0/connpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-14 14:48:44.000000 connpy-3.0.0/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-14 14:48:44.000000 connpy-3.0.0/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-14 14:48:44.000000 connpy-3.0.0/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47147 2023-04-14 14:48:44.000000 connpy-3.0.0/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27912 2023-04-14 14:48:44.000000 connpy-3.0.0/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:48:54.647227 connpy-3.0.0/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 14:48:54.000000 connpy-3.0.0/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 14:48:54.000000 connpy-3.0.0/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:48:54.000000 connpy-3.0.0/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 14:48:54.000000 connpy-3.0.0/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 14:48:54.000000 connpy-3.0.0/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 14:48:54.000000 connpy-3.0.0/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-14 14:48:54.647227 connpy-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 14:48:44.000000 connpy-3.0.0/setup.py
```

### Comparing `connpy-2.1.8/LICENSE` & `connpy-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-2.1.8/PKG-INFO` & `connpy-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 2.1.8
+Version: 3.0.0
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-2.1.8/README.md` & `connpy-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `connpy-2.1.8/connpy/__init__.py` & `connpy-3.0.0/connpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,80 @@
-#!/usr/bin/env python3
-'''
-## Connection manager
+Metadata-Version: 2.1
+Name: connpy
+Version: 3.0.0
+Summary: Connpy is a SSH/Telnet connection manager and automation module
+Home-page: https://github.com/fluzzi/connpy
+Author: Federico Luzzi
+Author-email: fluzzi@gmail.com
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
+Project-URL: Documentation, https://fluzzi.github.io/connpy/
+Keywords: networking,automation,ssh,telnet,connection manager
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: System :: Networking
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Programming Language :: Python :: 3
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Description-Content-Type: text/markdown
+Provides-Extra: fuzzysearch
+License-File: LICENSE
+
+# Conn
+[![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
+[![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
+[![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
+[![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 
-Connpy is a connection manager that allows you to store nodes to connect them fast and password free.
+Connpy is a ssh and telnet connection manager and automation module
 
-### Features
-    - You can generate profiles and reference them from nodes using @profilename 
-      so you dont need to edit multiple nodes when changing password or other 
-      information.
-    - Nodes can be stored on @folder or @subfolder@folder to organize your 
-      devices. Then can be referenced using node@subfolder@folder or node@folder
-    - If you have too many nodes. Get completion script using: conn config 
-      --completion, or use fzf installing pyfzf and running conn config --fzf true
-    - Much more!
+## Installation
 
-### Usage
-```
-usage: conn [-h] [--add | --del | --mod | --show | --debug] [node|folder]
-       conn {profile,move,mv,copy,cp,list,ls,bulk,config} ...
-
-positional arguments:
-  node|folder    node[@subfolder][@folder]
-                 Connect to specific node or show all matching nodes
-                 [@subfolder][@folder]
-                 Show all available connections globaly or in specified path
-Options:
-  -h, --help         show this help message and exit
-  -v, --version      Show version
-  -a, --add          Add new node[@subfolder][@folder] or [@subfolder]@folder
-  -r, --del, --rm    Delete node[@subfolder][@folder] or [@subfolder]@folder
-  -e, --mod, --edit  Modify node[@subfolder][@folder]
-  -s, --show         Show node[@subfolder][@folder]
-  -d, --debug        Display all conections steps
-
-Commands:
-  profile        Manage profiles
-  move (mv)      Move node
-  copy (cp)      Copy node
-  list (ls)      List profiles, nodes or folders
-  bulk           Add nodes in bulk
-  run            Run scripts or commands on nodes
-  config         Manage app config
-```
-
-###   Manage profiles
-```
-usage: conn profile [-h] (--add | --del | --mod | --show) profile
-
-positional arguments:
-  profile        Name of profile to manage
-
-options:
-  -h, --help         show this help message and exit
-  -a, --add          Add new profile
-  -r, --del, --rm    Delete profile
-  -e, --mod, --edit  Modify profile
-  -s, --show         Show profile
-
-```
-
-###   Examples
-```
-   conn profile --add office-user
-   conn --add @office
-   conn --add @datacenter@office
-   conn --add server@datacenter@office
-   conn --add pc@office
-   conn --show server@datacenter@office
-   conn pc@office
-   conn server
-``` 
-
-## Automation module
-the automation module
+pip install connpy
 
+## Automation module usage
 ### Standalone module
 ```
 import connpy
-router = connpy.node("unique name","ip/hostname", user="user", password="pass")
+router = connpy.node("unique name","ip/hostname", user="username", password="password")
 router.run(["term len 0","show run"])
 print(router.output)
 hasip = router.test("show ip int brief","1.1.1.1")
 if hasip:
     print("Router has ip 1.1.1.1")
 else:
     print("router does not have ip 1.1.1.1")
 ```
 
 ### Using manager configuration
 ```
 import connpy
 conf = connpy.configfile()
-device = conf.getitem("server@office")
-server = connpy.node("unique name", **device, config=conf)
-result = server.run(["cd /", "ls -la"])
+device = conf.getitem("router@office")
+router = connpy.node("unique name", **device, config=conf)
+result = router.run("show ip int brief")
 print(result)
 ```
-### Running parallel tasks 
+### Running parallel tasks on multiple devices 
 ```
 import connpy
 conf = connpy.configfile()
 #You can get the nodes from the config from a folder and fitlering in it
 nodes = conf.getitem("@office", ["router1", "router2", "router3"])
 #You can also get each node individually:
 nodes = {}
 nodes["router1"] = conf.getitem("router1@office")
 nodes["router2"] = conf.getitem("router2@office")
 nodes["router10"] = conf.getitem("router10@datacenter")
 #Also, you can create the nodes manually:
 nodes = {}
-nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "pass1"}
-nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "pass2"}
-nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "pass3"}
+nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "password1"}
+nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "password2"}
+nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "password3"}
 #Finally you run some tasks on the nodes
 mynodes = connpy.nodes(nodes, config = conf)
 result = mynodes.test(["show ip int br"], "1.1.1.2")
 for i in result:
     print("---" + i + "---")
     print(result[i])
     print()
@@ -141,20 +100,79 @@
 expected = "!"
 routers = connpy.nodes(nodes, config = config)
 routers.run(commands, variables)
 routers.test("ping {ip}", expected, variables)
 for key in routers.result:
     print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
 ```
-'''
-from .core import node,nodes
-from .configfile import configfile
-from .connapp import connapp
-from ._version import __version__
-from pkg_resources import get_distribution
-
-__all__ = ["node", "nodes", "configfile", "connapp"]
-__author__ = "Federico Luzzi"
-__pdoc__ = {
-    'core': False,
-    'completion': False,
-}
+
+## Connection manager 
+### Features
+    - You can generate profiles and reference them from nodes using @profilename so you dont
+      need to edit multiple nodes when changing password or other information.
+    - Nodes can be stored on @folder or @subfolder@folder to organize your devices. Then can 
+      be referenced using node@subfolder@folder or node@folder
+    - If you have too many nodes. Get completion script using: conn config --completion.
+      Or use fzf installing pyfzf and running conn config --fzf true
+    - Much more!
+
+### Usage:
+```
+usage: conn [-h] [--add | --del | --mod | --show | --debug] [node|folder]
+       conn {profile,move,mv,copy,cp,list,ls,bulk,config} ...
+
+positional arguments:
+  node|folder    node[@subfolder][@folder]
+                 Connect to specific node or show all matching nodes
+                 [@subfolder][@folder]
+                 Show all available connections globaly or in specified path
+```
+
+### Options:
+```
+  -h, --help         show this help message and exit
+  -v, --version      Show version
+  -a, --add          Add new node[@subfolder][@folder] or [@subfolder]@folder
+  -r, --del, --rm    Delete node[@subfolder][@folder] or [@subfolder]@folder
+  -e, --mod, --edit  Modify node[@subfolder][@folder]
+  -s, --show         Show node[@subfolder][@folder]
+  -d, --debug        Display all conections steps
+```
+
+### Commands:
+```
+  profile        Manage profiles
+  move (mv)      Move node
+  copy (cp)      Copy node
+  list (ls)      List profiles, nodes or folders
+  bulk           Add nodes in bulk
+  run            Run scripts or commands on nodes
+  config         Manage app config
+```
+
+### Manage profiles:
+```
+usage: conn profile [-h] (--add | --del | --mod | --show) profile
+
+positional arguments:
+  profile        Name of profile to manage
+
+options:
+  -h, --help         show this help message and exit
+  -a, --add          Add new profile
+  -r, --del, --rm    Delete profile
+  -e, --mod, --edit  Modify profile
+  -s, --show         Show profile
+
+```
+
+### Examples:
+```
+   conn profile --add office-user
+   conn --add @office
+   conn --add @datacenter@office
+   conn --add server@datacenter@office
+   conn --add pc@office
+   conn --show server@datacenter@office
+   conn pc@office
+   conn server
+```
```

### Comparing `connpy-2.1.8/connpy/completion.py` & `connpy-3.0.0/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-2.1.8/connpy/configfile.py` & `connpy-3.0.0/connpy/configfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,17 +45,25 @@
 
             - key  (str): Path/file to RSA key file. If left empty default
                           path is ~/.config/conn/.osk
 
         '''
         home = os.path.expanduser("~")
         defaultdir = home + '/.config/conn'
-        defaultfile = defaultdir + '/config.json'
-        defaultkey = defaultdir + '/.osk'
         Path(defaultdir).mkdir(parents=True, exist_ok=True)
+        pathfile = defaultdir + '/.folder'
+        try:
+            with open(pathfile, "r") as f:
+                configdir = f.read().strip()
+        except:
+            with open(pathfile, "w") as f:
+                f.write(str(defaultdir))
+            configdir = defaultdir
+        defaultfile = configdir + '/config.json'
+        defaultkey = configdir + '/.osk'
         if conf == None:
             self.file = defaultfile
         else:
             self.file = conf
         if key == None:
             self.key = defaultkey
         else:
@@ -229,7 +237,48 @@
         #Add profile from config
         self.profiles[id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user}
             
 
     def _profiles_del(self,*, id ):
         #Delete profile from config
         del self.profiles[id]
+        
+    def _getallnodes(self):
+        #get all nodes on configfile
+        nodes = []
+        layer1 = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "connection"]
+        folders = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
+        nodes.extend(layer1)
+        for f in folders:
+            layer2 = [k + "@" + f for k,v in self.connections[f].items() if isinstance(v, dict) and v["type"] == "connection"]
+            nodes.extend(layer2)
+            subfolders = [k for k,v in self.connections[f].items() if isinstance(v, dict) and v["type"] == "subfolder"]
+            for s in subfolders:
+                layer3 = [k + "@" + s + "@" + f for k,v in self.connections[f][s].items() if isinstance(v, dict) and v["type"] == "connection"]
+                nodes.extend(layer3)
+        return nodes
+
+    def _getallfolders(self):
+        #get all folders on configfile
+        folders = ["@" + k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
+        subfolders = []
+        for f in folders:
+            s = ["@" + k + f for k,v in self.connections[f[1:]].items() if isinstance(v, dict) and v["type"] == "subfolder"]
+            subfolders.extend(s)
+        folders.extend(subfolders)
+        return folders
+
+    def _profileused(self, profile):
+        #Check if profile is used before deleting it
+        nodes = []
+        layer1 = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "connection" and ("@" + profile in v.values() or ( isinstance(v["password"],list) and "@" + profile in v["password"]))]
+        folders = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
+        nodes.extend(layer1)
+        for f in folders:
+            layer2 = [k + "@" + f for k,v in self.connections[f].items() if isinstance(v, dict) and v["type"] == "connection" and ("@" + profile in v.values() or ( isinstance(v["password"],list) and "@" + profile in v["password"]))]
+            nodes.extend(layer2)
+            subfolders = [k for k,v in self.connections[f].items() if isinstance(v, dict) and v["type"] == "subfolder"]
+            for s in subfolders:
+                layer3 = [k + "@" + s + "@" + f for k,v in self.connections[f][s].items() if isinstance(v, dict) and v["type"] == "connection" and ("@" + profile in v.values() or ( isinstance(v["password"],list) and "@" + profile in v["password"]))]
+                nodes.extend(layer3)
+        return nodes
+
```

### Comparing `connpy-2.1.8/connpy/connapp.py` & `connpy-3.0.0/connpy/connapp.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 from Crypto.Cipher import PKCS1_OAEP
 import ast
 import argparse
 import sys
 import inquirer
 from .core import node,nodes
 from ._version import __version__
+from .api import *
 import yaml
 try:
     from pyfzf.pyfzf import FzfPrompt
 except:
     FzfPrompt = None
+home = os.path.expanduser("~")
+defaultdir = home + '/.config/conn'
+
 
 
 #functions and classes
 
 class connapp:
     ''' This class starts the connection manager app. It's normally used by connection manager but you can use it on a script to run the connection manager your way and use a different configfile and key.
         '''
@@ -32,16 +36,16 @@
                             the nodes configuration and the methods to manage
                             the config file.
 
         '''
         self.node = node
         self.connnodes = nodes
         self.config = config
-        self.nodes = self._getallnodes()
-        self.folders = self._getallfolders()
+        self.nodes = self.config._getallnodes()
+        self.folders = self.config._getallfolders()
         self.profiles = list(self.config.profiles.keys())
         self.case = self.config.config["case"]
         try:
             self.fzf = self.config.config["fzf"]
         except:
             self.fzf = False
 
@@ -95,24 +99,32 @@
         bulkparser.add_argument("bulk", const="bulk", nargs=0, action=self._store_type, help="Add nodes in bulk")
         bulkparser.set_defaults(func=self._func_others)
         #RUNPARSER
         runparser = subparsers.add_parser("run", help="Run scripts or commands on nodes", formatter_class=argparse.RawTextHelpFormatter) 
         runparser.add_argument("run", nargs='+', action=self._store_type, help=self._help("run"), default="run")
         runparser.add_argument("-g","--generate", dest="action", action="store_const", help="Generate yaml file template", const="generate", default="run")
         runparser.set_defaults(func=self._func_run)
+        #APIPARSER
+        apiparser = subparsers.add_parser("api", help="Start and stop connpy api") 
+        apicrud = apiparser.add_mutually_exclusive_group(required=True)
+        apicrud.add_argument("--start", dest="start", nargs=0, action=self._store_type, help="Start conppy api")
+        apicrud.add_argument("--restart", dest="restart", nargs=0, action=self._store_type, help="Restart conppy api")
+        apicrud.add_argument("--stop", dest="stop", nargs=0, action=self._store_type, help="Stop conppy api")
+        apiparser.set_defaults(func=self._func_api)
         #CONFIGPARSER
         configparser = subparsers.add_parser("config", help="Manage app config") 
         configcrud = configparser.add_mutually_exclusive_group(required=True)
         configcrud.add_argument("--allow-uppercase", dest="case", nargs=1, action=self._store_type, help="Allow case sensitive names", choices=["true","false"])
         configcrud.add_argument("--fzf", dest="fzf", nargs=1, action=self._store_type, help="Use fzf for lists", choices=["true","false"])
         configcrud.add_argument("--keepalive", dest="idletime", nargs=1, action=self._store_type, help="Set keepalive time in seconds, 0 to disable", type=int, metavar="INT")
         configcrud.add_argument("--completion", dest="completion", nargs=1, choices=["bash","zsh"], action=self._store_type, help="Get terminal completion configuration for conn")
+        configcrud.add_argument("--configfolder", dest="configfolder", nargs=1, action=self._store_type, help="Set the default location for config file", metavar="FOLDER")
         configparser.set_defaults(func=self._func_others)
         #Manage sys arguments
-        commands = ["node", "profile", "mv", "move","copy", "cp", "bulk", "ls", "list", "run", "config"]
+        commands = ["node", "profile", "mv", "move","copy", "cp", "bulk", "ls", "list", "run", "config", "api"]
         profilecmds = ["--add", "-a", "--del", "--rm",  "-r", "--mod", "--edit", "-e", "--show", "-s"]
         if len(argv) >= 2 and argv[1] == "profile" and argv[0] in profilecmds:
             argv[1] = argv[0]
             argv[0] = "profile"
         if len(argv) < 1 or argv[0] not in commands:
             argv.insert(0,"node")
         args = defaultparser.parse_args(argv)
@@ -293,15 +305,15 @@
         matches = list(filter(lambda k: k == args.data[0], self.profiles))
         if len(matches) == 0:
             print("{} not found".format(args.data[0]))
             exit(2)
         if matches[0] == "default":
             print("Can't delete default profile")
             exit(6)
-        usedprofile = self._profileused(matches[0])
+        usedprofile = self.config._profileused(matches[0])
         if len(usedprofile) > 0:
             print("Profile {} used in the following nodes:".format(matches[0]))
             print(", ".join(usedprofile))
             exit(8)
         question = [inquirer.Confirm("delete", message="Are you sure you want to delete {}?".format(matches[0]))]
         confirm = inquirer.prompt(question)
         if confirm["delete"]:
@@ -355,15 +367,15 @@
         else:
             self.config._profiles_add(**updateprofile)
             self.config._saveconfig(self.config.file)
             print("{} edited succesfully".format(args.data[0]))
     
     def _func_others(self, args):
         #Function called when using other commands
-        actions = {"ls": self._ls, "move": self._mvcp, "cp": self._mvcp, "bulk": self._bulk, "completion": self._completion, "case": self._case, "fzf": self._fzf, "idletime": self._idletime}
+        actions = {"ls": self._ls, "move": self._mvcp, "cp": self._mvcp, "bulk": self._bulk, "completion": self._completion, "case": self._case, "fzf": self._fzf, "idletime": self._idletime, "configfolder": self._configfolder}
         return actions.get(args.command)(args)
 
     def _ls(self, args):
         print(*getattr(self, args.data), sep="\n")
 
     def _mvcp(self, args):
         if not self.case:
@@ -429,15 +441,15 @@
             newnode["port"] = newnodes["port"]
             newnode["options"] = newnodes["options"]
             newnode["logs"] = newnodes["logs"]
             newnode["user"] = newnodes["user"]
             newnode["password"] = newnodes["password"]
             count +=1
             self.config._connections_add(**newnode)
-            self.nodes = self._getallnodes()
+            self.nodes = self.config._getallnodes()
         if count > 0:
             self.config._saveconfig(self.config.file)
             print("Succesfully added {} nodes".format(count))
         else:
             print("0 nodes added")
 
     def _completion(self, args):
@@ -461,25 +473,42 @@
         self._change_settings(args.command, args.data[0])
 
     def _idletime(self, args):
         if args.data[0] < 0:
             args.data[0] = 0
         self._change_settings(args.command, args.data[0])
 
+    def _configfolder(self, args):
+        if not os.path.isdir(args.data[0]):
+            raise argparse.ArgumentTypeError(f"readable_dir:{args.data[0]} is not a valid path")
+        else:
+            pathfile = defaultdir + "/.folder"
+            folder = os.path.abspath(args.data[0]).rstrip('/')
+            with open(pathfile, "w") as f:
+                f.write(str(folder))
+            print("Config saved")
+
     def _change_settings(self, name, value):
         self.config.config[name] = value
         self.config._saveconfig(self.config.file)
         print("Config saved")
 
     def _func_run(self, args):
         if len(args.data) > 1:
             args.action = "noderun"
         actions = {"noderun": self._node_run, "generate": self._yaml_generate, "run": self._yaml_run}
         return actions.get(args.action)(args)
 
+    def _func_api(self, args):
+        if args.command == "stop" or args.command == "restart":
+            stop_api()
+        if args.command == "start" or args.command == "restart":
+            start_api()
+        return
+
     def _node_run(self, args):
         command = " ".join(args.data[1:])
         command = command.split("-")
         matches = list(filter(lambda k: k == args.data[0], self.nodes))
         if len(matches) == 0:
             print("{} not found".format(args.data[0]))
             exit(2)
@@ -862,15 +891,15 @@
     def _help(self, type):
         #Store text for help and other commands
         if type == "node":
             return "node[@subfolder][@folder]\nConnect to specific node or show all matching nodes\n[@subfolder][@folder]\nShow all available connections globaly or in specified path"
         if type == "usage":
             return "conn [-h] [--add | --del | --mod | --show | --debug] [node|folder]\n       conn {profile,move,mv,copy,cp,list,ls,bulk,config} ..."
         if type == "end":
-            return "Commands:\n  profile        Manage profiles\n  move (mv)      Move node\n  copy (cp)      Copy node\n  list (ls)      List profiles, nodes or folders\n  bulk           Add nodes in bulk\n  run            Run scripts or commands on nodes\n  config         Manage app config"
+            return "Commands:\n  profile        Manage profiles\n  move (mv)      Move node\n  copy (cp)      Copy node\n  list (ls)      List profiles, nodes or folders\n  bulk           Add nodes in bulk\n  run            Run scripts or commands on nodes\n  config         Manage app config\n  api            Start and stop connpy api"
         if type == "bashcompletion":
             return '''
 #Here starts bash completion for conn
 _conn()
 {
         strings="$(connpy-completion-helper ${#COMP_WORDS[@]} ${COMP_WORDS[@]})"
         COMPREPLY=($(compgen -W "$strings" -- "${COMP_WORDS[-1]}"))
@@ -962,54 +991,14 @@
     vrouter1@aws:
       id: 4
     vrouterN@aws:
       id: 5
   output: null
 ...'''
 
-    def _getallnodes(self):
-        #get all nodes on configfile
-        nodes = []
-        layer1 = [k for k,v in self.config.connections.items() if isinstance(v, dict) and v["type"] == "connection"]
-        folders = [k for k,v in self.config.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
-        nodes.extend(layer1)
-        for f in folders:
-            layer2 = [k + "@" + f for k,v in self.config.connections[f].items() if isinstance(v, dict) and v["type"] == "connection"]
-            nodes.extend(layer2)
-            subfolders = [k for k,v in self.config.connections[f].items() if isinstance(v, dict) and v["type"] == "subfolder"]
-            for s in subfolders:
-                layer3 = [k + "@" + s + "@" + f for k,v in self.config.connections[f][s].items() if isinstance(v, dict) and v["type"] == "connection"]
-                nodes.extend(layer3)
-        return nodes
-
-    def _getallfolders(self):
-        #get all folders on configfile
-        folders = ["@" + k for k,v in self.config.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
-        subfolders = []
-        for f in folders:
-            s = ["@" + k + f for k,v in self.config.connections[f[1:]].items() if isinstance(v, dict) and v["type"] == "subfolder"]
-            subfolders.extend(s)
-        folders.extend(subfolders)
-        return folders
-
-    def _profileused(self, profile):
-        #Check if profile is used before deleting it
-        nodes = []
-        layer1 = [k for k,v in self.config.connections.items() if isinstance(v, dict) and v["type"] == "connection" and ("@" + profile in v.values() or ( isinstance(v["password"],list) and "@" + profile in v["password"]))]
-        folders = [k for k,v in self.config.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
-        nodes.extend(layer1)
-        for f in folders:
-            layer2 = [k + "@" + f for k,v in self.config.connections[f].items() if isinstance(v, dict) and v["type"] == "connection" and ("@" + profile in v.values() or ( isinstance(v["password"],list) and "@" + profile in v["password"]))]
-            nodes.extend(layer2)
-            subfolders = [k for k,v in self.config.connections[f].items() if isinstance(v, dict) and v["type"] == "subfolder"]
-            for s in subfolders:
-                layer3 = [k + "@" + s + "@" + f for k,v in self.config.connections[f][s].items() if isinstance(v, dict) and v["type"] == "connection" and ("@" + profile in v.values() or ( isinstance(v["password"],list) and "@" + profile in v["password"]))]
-                nodes.extend(layer3)
-        return nodes
-
     def encrypt(self, password, keyfile=None):
         '''
         Encrypts password using RSA keyfile
 
         ### Parameters:  
 
             - password (str): Plaintext password to encrypt.
```

### Comparing `connpy-2.1.8/connpy/core.py` & `connpy-3.0.0/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-2.1.8/connpy.egg-info/PKG-INFO` & `connpy-3.0.0/connpy/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,177 @@
-Metadata-Version: 2.1
-Name: connpy
-Version: 2.1.8
-Summary: Connpy is a SSH/Telnet connection manager and automation module
-Home-page: https://github.com/fluzzi/connpy
-Author: Federico Luzzi
-Author-email: fluzzi@gmail.com
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
-Project-URL: Documentation, https://fluzzi.github.io/connpy/
-Keywords: networking,automation,ssh,telnet,connection manager
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: System :: Networking
-Classifier: Intended Audience :: Telecommunications Industry
-Classifier: Programming Language :: Python :: 3
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
-Provides-Extra: fuzzysearch
-License-File: LICENSE
-
-# Conn
-[![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
-[![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
-[![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
-[![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
+#!/usr/bin/env python3
+'''
+## Connection manager
 
-Connpy is a ssh and telnet connection manager and automation module
+Connpy is a connection manager that allows you to store nodes to connect them fast and password free.
 
-## Installation
+### Features
+    - You can generate profiles and reference them from nodes using @profilename 
+      so you dont need to edit multiple nodes when changing password or other 
+      information.
+    - Nodes can be stored on @folder or @subfolder@folder to organize your 
+      devices. Then can be referenced using node@subfolder@folder or node@folder
+    - If you have too many nodes. Get completion script using: conn config 
+      --completion, or use fzf installing pyfzf and running conn config --fzf true
+    - Much more!
+
+### Usage
+```
+usage: conn [-h] [--add | --del | --mod | --show | --debug] [node|folder]
+       conn {profile,move,mv,copy,cp,list,ls,bulk,config} ...
+
+positional arguments:
+  node|folder    node[@subfolder][@folder]
+                 Connect to specific node or show all matching nodes
+                 [@subfolder][@folder]
+                 Show all available connections globaly or in specified path
+Options:
+  -h, --help         show this help message and exit
+  -v, --version      Show version
+  -a, --add          Add new node[@subfolder][@folder] or [@subfolder]@folder
+  -r, --del, --rm    Delete node[@subfolder][@folder] or [@subfolder]@folder
+  -e, --mod, --edit  Modify node[@subfolder][@folder]
+  -s, --show         Show node[@subfolder][@folder]
+  -d, --debug        Display all conections steps
+
+Commands:
+  profile        Manage profiles
+  move (mv)      Move node
+  copy (cp)      Copy node
+  list (ls)      List profiles, nodes or folders
+  bulk           Add nodes in bulk
+  run            Run scripts or commands on nodes
+  config         Manage app config
+  api            Start and stop connpy api
+```
+
+###   Manage profiles
+```
+usage: conn profile [-h] (--add | --del | --mod | --show) profile
+
+positional arguments:
+  profile        Name of profile to manage
+
+options:
+  -h, --help         show this help message and exit
+  -a, --add          Add new profile
+  -r, --del, --rm    Delete profile
+  -e, --mod, --edit  Modify profile
+  -s, --show         Show profile
+
+```
+
+###   Examples
+```
+   conn profile --add office-user
+   conn --add @office
+   conn --add @datacenter@office
+   conn --add server@datacenter@office
+   conn --add pc@office
+   conn --show server@datacenter@office
+   conn pc@office
+   conn server
+``` 
+## http API
+With the Connpy API you can run commands on devices using http requests
+
+### 1. List Nodes
+
+**Endpoint**: `/list_nodes`
+
+**Method**: `POST`
+
+**Description**: This route returns a list of nodes. It can also filter the list based on a given keyword.
+
+#### Request Body:
+
+```json
+{
+  "filter": "<keyword>"
+}
+```
+
+* `filter` (optional): A keyword to filter the list of nodes. It returns only the nodes that contain the keyword. If not provided, the route will return the entire list of nodes.
+
+#### Response:
+
+- A JSON array containing the filtered list of nodes.
+
+---
+
+### 2. Run Commands
+
+**Endpoint**: `/run_commands`
 
-pip install connpy
+**Method**: `POST`
+
+**Description**: This route runs commands on selected nodes based on the provided action, nodes, and commands. It also supports executing tests by providing expected results.
+
+#### Request Body:
+
+```json
+{
+  "action": "<action>",
+  "nodes": "<nodes>",
+  "commands": "<commands>",
+  "expected": "<expected>",
+  "options": "<options>"
+}
+```
+
+* `action` (required): The action to be performed. Possible values: `run` or `test`.
+* `nodes` (required): A list of nodes or a single node on which the commands will be executed. The nodes can be specified as individual node names or a node group with the `@` prefix. Node groups can also be specified as arrays with a list of nodes inside the group.
+* `commands` (required): A list of commands to be executed on the specified nodes.
+* `expected` (optional, only used when the action is `test`): A single expected result for the test.
+* `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
+
+#### Response:
+
+- A JSON object with the results of the executed commands on the nodes.
+## Automation module
+the automation module
 
-## Automation module usage
 ### Standalone module
 ```
 import connpy
-router = connpy.node("unique name","ip/hostname", user="username", password="password")
+router = connpy.node("unique name","ip/hostname", user="user", password="pass")
 router.run(["term len 0","show run"])
 print(router.output)
 hasip = router.test("show ip int brief","1.1.1.1")
 if hasip:
     print("Router has ip 1.1.1.1")
 else:
     print("router does not have ip 1.1.1.1")
 ```
 
 ### Using manager configuration
 ```
 import connpy
 conf = connpy.configfile()
-device = conf.getitem("router@office")
-router = connpy.node("unique name", **device, config=conf)
-result = router.run("show ip int brief")
+device = conf.getitem("server@office")
+server = connpy.node("unique name", **device, config=conf)
+result = server.run(["cd /", "ls -la"])
 print(result)
 ```
-### Running parallel tasks on multiple devices 
+### Running parallel tasks 
 ```
 import connpy
 conf = connpy.configfile()
 #You can get the nodes from the config from a folder and fitlering in it
 nodes = conf.getitem("@office", ["router1", "router2", "router3"])
 #You can also get each node individually:
 nodes = {}
 nodes["router1"] = conf.getitem("router1@office")
 nodes["router2"] = conf.getitem("router2@office")
 nodes["router10"] = conf.getitem("router10@datacenter")
 #Also, you can create the nodes manually:
 nodes = {}
-nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "password1"}
-nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "password2"}
-nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "password3"}
+nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "pass1"}
+nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "pass2"}
+nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "pass3"}
 #Finally you run some tasks on the nodes
 mynodes = connpy.nodes(nodes, config = conf)
 result = mynodes.test(["show ip int br"], "1.1.1.2")
 for i in result:
     print("---" + i + "---")
     print(result[i])
     print()
@@ -100,79 +197,21 @@
 expected = "!"
 routers = connpy.nodes(nodes, config = config)
 routers.run(commands, variables)
 routers.test("ping {ip}", expected, variables)
 for key in routers.result:
     print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
 ```
-
-## Connection manager 
-### Features
-    - You can generate profiles and reference them from nodes using @profilename so you dont
-      need to edit multiple nodes when changing password or other information.
-    - Nodes can be stored on @folder or @subfolder@folder to organize your devices. Then can 
-      be referenced using node@subfolder@folder or node@folder
-    - If you have too many nodes. Get completion script using: conn config --completion.
-      Or use fzf installing pyfzf and running conn config --fzf true
-    - Much more!
-
-### Usage:
-```
-usage: conn [-h] [--add | --del | --mod | --show | --debug] [node|folder]
-       conn {profile,move,mv,copy,cp,list,ls,bulk,config} ...
-
-positional arguments:
-  node|folder    node[@subfolder][@folder]
-                 Connect to specific node or show all matching nodes
-                 [@subfolder][@folder]
-                 Show all available connections globaly or in specified path
-```
-
-### Options:
-```
-  -h, --help         show this help message and exit
-  -v, --version      Show version
-  -a, --add          Add new node[@subfolder][@folder] or [@subfolder]@folder
-  -r, --del, --rm    Delete node[@subfolder][@folder] or [@subfolder]@folder
-  -e, --mod, --edit  Modify node[@subfolder][@folder]
-  -s, --show         Show node[@subfolder][@folder]
-  -d, --debug        Display all conections steps
-```
-
-### Commands:
-```
-  profile        Manage profiles
-  move (mv)      Move node
-  copy (cp)      Copy node
-  list (ls)      List profiles, nodes or folders
-  bulk           Add nodes in bulk
-  run            Run scripts or commands on nodes
-  config         Manage app config
-```
-
-### Manage profiles:
-```
-usage: conn profile [-h] (--add | --del | --mod | --show) profile
-
-positional arguments:
-  profile        Name of profile to manage
-
-options:
-  -h, --help         show this help message and exit
-  -a, --add          Add new profile
-  -r, --del, --rm    Delete profile
-  -e, --mod, --edit  Modify profile
-  -s, --show         Show profile
-
-```
-
-### Examples:
-```
-   conn profile --add office-user
-   conn --add @office
-   conn --add @datacenter@office
-   conn --add server@datacenter@office
-   conn --add pc@office
-   conn --show server@datacenter@office
-   conn pc@office
-   conn server
-``` 
+'''
+from .core import node,nodes
+from .configfile import configfile
+from .connapp import connapp
+from ._version import __version__
+from pkg_resources import get_distribution
+
+__all__ = ["node", "nodes", "configfile", "connapp"]
+__author__ = "Federico Luzzi"
+__pdoc__ = {
+    'core': False,
+    'completion': False,
+    'api': False
+}
```

### Comparing `connpy-2.1.8/setup.cfg` & `connpy-3.0.0/setup.cfg`

 * *Files identical despite different names*

