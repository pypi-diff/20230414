# Comparing `tmp/TapisCL-ICICLE-0.0.23.tar.gz` & `tmp/TapisCL-ICICLE-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.23.tar", last modified: Thu Apr 13 04:40:54 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.24.tar", last modified: Fri Apr 14 16:59:01 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.23.tar` & `TapisCL-ICICLE-0.0.24.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 04:40:54.013614 TapisCL-ICICLE-0.0.23/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/LICENSE
--rw-rw-rw-   0        0        0    43856 2023-04-13 04:40:54.012595 TapisCL-ICICLE-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0     1946 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 04:40:54.003737 TapisCL-ICICLE-0.0.23/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1408 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    11151 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     6873 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     4985 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     1049 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10512 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    18336 2023-04-13 04:36:57.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 04:40:54.011093 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    43856 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-04-13 04:40:14.000000 TapisCL-ICICLE-0.0.23/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 04:40:54.013614 TapisCL-ICICLE-0.0.23/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 16:59:01.760559 TapisCL-ICICLE-0.0.24/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/LICENSE
+-rw-rw-rw-   0        0        0    43887 2023-04-14 16:59:01.759563 TapisCL-ICICLE-0.0.24/PKG-INFO
+-rw-rw-rw-   0        0        0     1977 2023-04-14 16:57:05.000000 TapisCL-ICICLE-0.0.24/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 16:59:01.751591 TapisCL-ICICLE-0.0.24/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1408 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    10875 2023-04-14 16:53:19.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     6873 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     4985 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     1049 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10368 2023-04-14 16:52:30.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    18336 2023-04-13 04:36:57.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:59:01.758566 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    43887 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-04-14 16:57:10.000000 TapisCL-ICICLE-0.0.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 16:59:01.760559 TapisCL-ICICLE-0.0.24/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.23/LICENSE` & `TapisCL-ICICLE-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.23/PKG-INFO` & `TapisCL-ICICLE-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.23
+Version: 0.0.24
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,15 +694,15 @@
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
-1. `pip install TapisCL-ICICLE`
+1. `pip install TapisCL-ICICLE`. Ensure your version is 0.0.24
 2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
 **Full Terminal Interface:**
```

### Comparing `TapisCL-ICICLE-0.0.23/README.md` & `TapisCL-ICICLE-0.0.24/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
-1. `pip install TapisCL-ICICLE`
+1. `pip install TapisCL-ICICLE`. Ensure your version is 0.0.24
 2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
 **Full Terminal Interface:**
```

### Comparing `TapisCL-ICICLE-0.0.23/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.24/TapisCLICICLE/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.23/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.24/TapisCLICICLE/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import sys
 import pyfiglet
 from getpass import getpass
 import os
 import time
 from pprint import pprint
 import json
-from TypeEnforcement.type_enforcer import TypeEnforcer
 
 try:
     from . import schemas
     from . import socketOpts as SO
     from . import helpers
     from . import decorators
     from . import args
@@ -28,15 +27,14 @@
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(__file__)))
 server_path = os.path.join(__location__, 'server.py')
 
 
 class CLI(SO.SocketOpts, helpers.OperationsHelper, decorators.DecoratorSetup, helpers.Formatters):
-    @TypeEnforcer.enforcer(recursive=True)
     def __init__(self, IP: str, PORT: int):
         self.ip, self.port = IP, PORT
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM) 
 
         # sets up connection with the server
         self.username, self.url = self.connect()
 
@@ -113,41 +111,37 @@
                     if verification.response_message[1] == 3:
                         sys.exit(0)
                     continue
 
         print(f"[+] Connected to the Tapis service at {connection_info.url}")
         return connection_info.username, connection_info.url # return the username and url
 
-    @TypeEnforcer.enforcer(recursive=True)
     def process_command(self, command: str) -> list[str]: 
         """
         split the command string into a list. Not sure why this was even made
         """
         command = command.strip().split(' ') 
         return command
 
-    @TypeEnforcer.enforcer(recursive=True)
     def expression_input(self) -> str: # for subclients. Pods and apps running through Tapis will have their own inputs. This gives user an interface
         print("Enter 'exit' to submit") # user must enter exit to submit their input
         expression = ''
         line = ''
         while line != 'exit': # handles multiple lines of input. Good for neo4j expressions
             line = str(input("> "))
             expression += line
         return expression
 
-    @TypeEnforcer.enforcer(recursive=True)
     def fillout_form(self, form: list) -> dict:
         filled_form = dict()
         for field in form:
             value = str(input(f"{field}: "))
             filled_form.update({field:value})
         return filled_form
 
-    @TypeEnforcer.enforcer(recursive=True)
     def command_operator(self, kwargs: dict | list, exit_: int=0): # parses command input
         if isinstance(kwargs, list): # check if the command input is from the CLI, or direct input
             kwargs = vars(self.parser.parse_args(kwargs)) # parse the arguments
         if not kwargs['command_group']:
             return False
         command = schemas.CommandData(kwargs = kwargs, exit_status = exit_)
         return command
```

### Comparing `TapisCL-ICICLE-0.0.23/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.24/TapisCLICICLE/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.23/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.24/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.23/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.24/TapisCLICICLE/helpers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.23/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.24/TapisCLICICLE/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.23/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.24/TapisCLICICLE/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import time
 import re
 from tapipy.tapis import Tapis
 import socket
 import os
 import logging
 from tapisObjectWrappers import Files, Apps, Pods, Systems, Neo4jCLI
-from TypeEnforcement.type_enforcer import TypeEnforcer
 import typing
 
 try:
     from . import exceptions
     from . import socketOpts as SO
     from . import helpers
     from . import schemas
@@ -20,15 +19,14 @@
     import exceptions
     import socketOpts as SO
     import helpers
     import schemas
     import decorators
 
 class Server(SO.SocketOpts, helpers.OperationsHelper, decorators.DecoratorSetup, helpers.DynamicHelpUtility):
-    @TypeEnforcer.enforcer(recursive=True)
     def __init__(self, IP: str, PORT: int):
         # logger setup
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(logging.INFO)
         stream_handler = logging.StreamHandler(stream=sys.stdout)
 
         file_handler = logging.FileHandler(
@@ -138,15 +136,14 @@
         self.url = url
         self.access_token = access_token
 
         self.logger.info(f"initiated in {time.time()-start}")
 
         return f"Successfully initialized tapis service on {self.url}"
 
-    @TypeEnforcer.enforcer(recursive=True)
     def accept(self, initial: bool=False):  # function to accept CLI connection to the server
         self.connection, ip_port = self.sock.accept()  # connection request is accepted
         self.logger.info("Received connection request")
 
         if initial:  # if this is the first time in the session that the cli is connecting
             startup_data = schemas.StartupData(initial = initial)
             self.json_send(startup_data.dict())
```

### Comparing `TapisCL-ICICLE-0.0.23/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.24/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.23/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.24/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.23
+Version: 0.0.24
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,15 +694,15 @@
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
-1. `pip install TapisCL-ICICLE`
+1. `pip install TapisCL-ICICLE`. Ensure your version is 0.0.24
 2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
 **Full Terminal Interface:**
```

### Comparing `TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.23/pyproject.toml` & `TapisCL-ICICLE-0.0.24/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.23"
+version = "0.0.24"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

