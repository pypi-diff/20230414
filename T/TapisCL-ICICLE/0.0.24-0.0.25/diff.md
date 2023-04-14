# Comparing `tmp/TapisCL-ICICLE-0.0.24.tar.gz` & `tmp/TapisCL-ICICLE-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.24.tar", last modified: Fri Apr 14 16:59:01 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.25.tar", last modified: Fri Apr 14 18:30:06 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.24.tar` & `TapisCL-ICICLE-0.0.25.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 16:59:01.760559 TapisCL-ICICLE-0.0.24/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/LICENSE
--rw-rw-rw-   0        0        0    43887 2023-04-14 16:59:01.759563 TapisCL-ICICLE-0.0.24/PKG-INFO
--rw-rw-rw-   0        0        0     1977 2023-04-14 16:57:05.000000 TapisCL-ICICLE-0.0.24/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 16:59:01.751591 TapisCL-ICICLE-0.0.24/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1408 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    10875 2023-04-14 16:53:19.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     6873 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     4985 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     1049 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10368 2023-04-14 16:52:30.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    18336 2023-04-13 04:36:57.000000 TapisCL-ICICLE-0.0.24/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:59:01.758566 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    43887 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 16:59:01.000000 TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-04-14 16:57:10.000000 TapisCL-ICICLE-0.0.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 16:59:01.760559 TapisCL-ICICLE-0.0.24/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 18:30:06.526605 TapisCL-ICICLE-0.0.25/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/LICENSE
+-rw-rw-rw-   0        0        0    43880 2023-04-14 18:30:06.526605 TapisCL-ICICLE-0.0.25/PKG-INFO
+-rw-rw-rw-   0        0        0     1970 2023-04-14 17:01:05.000000 TapisCL-ICICLE-0.0.25/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 18:30:06.519628 TapisCL-ICICLE-0.0.25/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1408 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    10911 2023-04-14 18:13:31.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     6873 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     5132 2023-04-14 18:06:28.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     1049 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10402 2023-04-14 18:00:07.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    18763 2023-04-14 18:25:04.000000 TapisCL-ICICLE-0.0.25/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:30:06.525608 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    43880 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 18:30:06.000000 TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-04-14 18:29:21.000000 TapisCL-ICICLE-0.0.25/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 18:30:06.526605 TapisCL-ICICLE-0.0.25/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.24/LICENSE` & `TapisCL-ICICLE-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.24/PKG-INFO` & `TapisCL-ICICLE-0.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.24
+Version: 0.0.25
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
-1. `pip install TapisCL-ICICLE`. Ensure your version is 0.0.24
+1. `pip install TapisCL-ICICLE`. Current version 0.0.24
 2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
 **Full Terminal Interface:**
```

### Comparing `TapisCL-ICICLE-0.0.24/README.md` & `TapisCL-ICICLE-0.0.25/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
-1. `pip install TapisCL-ICICLE`. Ensure your version is 0.0.24
+1. `pip install TapisCL-ICICLE`. Current version 0.0.24
 2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
 **Full Terminal Interface:**
```

### Comparing `TapisCL-ICICLE-0.0.24/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.25/TapisCLICICLE/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.24/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.25/TapisCLICICLE/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,16 @@
                     startup_flag = True # set the flag to true so the thread runs only once
                     continue
 
     def connect(self):
         """
         connect to the local server
         """
-        self.connection_initialization() # connect to the server
-        #self.connection.connect((self.ip, self.port)) # enable me for debugging. Requires manual server start
+        #self.connection_initialization() # connect to the server
+        self.connection.connect((self.ip, self.port)) # enable me for debugging. Requires manual server start
         connection_info: schemas.StartupData = self.schema_unpack() # receive info from the server whether it is a first time connection
         if connection_info.initial: # if the server is receiving its first connection for the session\
             while True:
                 try:
                     url = str(input("\nEnter the link for the tapis service you are connecting to: ")).strip()
                 except KeyboardInterrupt:
                     url = " "
@@ -124,15 +124,16 @@
 
     def expression_input(self) -> str: # for subclients. Pods and apps running through Tapis will have their own inputs. This gives user an interface
         print("Enter 'exit' to submit") # user must enter exit to submit their input
         expression = ''
         line = ''
         while line != 'exit': # handles multiple lines of input. Good for neo4j expressions
             line = str(input("> "))
-            expression += line
+            if line != 'exit':
+                expression += line
         return expression
 
     def fillout_form(self, form: list) -> dict:
         filled_form = dict()
         for field in form:
             value = str(input(f"{field}: "))
             filled_form.update({field:value})
```

### Comparing `TapisCL-ICICLE-0.0.24/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.25/TapisCLICICLE/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.24/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.25/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.24/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.25/TapisCLICICLE/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,17 @@
     return args
 
 class OperationsHelper:
     def filter_kwargs(self, func: typing.Callable, kwargs: dict) -> dict:
         filtered = dict()
         variables = list(get_parameters(func))
         for arg in variables:
-            if arg != "password": filtered.update({arg:kwargs[arg]})
-            else: filtered.update({'password':None})
+            if arg != "password" and arg != "expression": filtered.update({arg:kwargs[arg]})
+            elif arg == "password": filtered.update({'password':None})
+            elif arg == "expression": filtered.update({'expression':None})
         return filtered
 
     def print_dict(self, dict_):
         for key, value in dict_.items():
             print(f"{key}: {value}")
     
 
@@ -64,15 +65,15 @@
                 if map == self.command_map:
                     argument_help = f"{command_name}"
                     arguments = get_parameters(command)
                 else:
                     argument_help = f"{command_name} -c help"
             if arguments:
                 for argument in arguments:
-                    if argument != "password" and argument != "description":
+                    if argument != "password" and argument != "description" and argument != "expression":
                         argument_help += f" {command_parameters[argument]['args'][1]} <{argument}>"
 
             command_help['syntax'] = argument_help
             help_menu[command_name] = command_help
         return help_menu
             
     def help_generation(self) -> dict:
```

### Comparing `TapisCL-ICICLE-0.0.24/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.25/TapisCLICICLE/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.24/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.25/TapisCLICICLE/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,21 +75,22 @@
 
         # instantiate the subsystems
         self.logger.info('initialization complete')
         self.command_group_map = {
             'pods':self.pods,
             'systems':self.systems,
             'files':self.files,
-            'apps':self.apps
+            'apps':self.apps,
         }
         self.command_map = {
             'help':self.help,
             'whoami':self.pods.whoami,
             'exit':self.__exit,
             'shutdown':self.__shutdown,
+            'neo4j':self.neo4j,
             'switch_service':self.tapis_init
         }
         help0, help1 = self.help_generation()
         self.help = dict(help0, **help1)
 
     @decorators.Auth
     def tapis_init(self, username: str, password: str, link: str) -> tuple[typing.Any, str, str] | None:  # link is the baseURL
```

### Comparing `TapisCL-ICICLE-0.0.24/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.25/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.24/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.25/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,29 @@
     def help(self, name: typing.Optional[str]):
         """
         @help: get help information for the command group
         """
         if name:
             return self.help[name]
         return self.help
+    
+
+class TapisQuery(tapisObject):
+    def __init__(self, tapis_object, uname, pword, connection):
+        super().__init__(tapis_object, uname, pword, connection)
+        self.t = tapis_object
+        self.__code__ = self.query.__code__
+
+    def __call__(self, **kwargs):
+        try:
+            kwargs = self.filter_kwargs(self.query, kwargs)
+            result = self.query(**kwargs)
+            return result
+        except (tapipy.errors.NotFoundError, tapipy.errors.BadRequestError, tapipy.errors.BaseTapyException) as e:
+            return str(e)
 
 
 class Systems(tapisObject):
     """
     @help: Access Tapis systems through the connected service
     """
     def __init__(self, tapis_instance, username, password, connection):
@@ -155,35 +170,33 @@
         """
         @help: delete the selected system
         """
         return_value = self.t.systems.deleteSystem(systemId=id)
         return return_value
 
 
-class Neo4jCLI(tapisObject):
-    def __init__(self, tapis_object, uname, pword, connection):
-        super().__init__(tapis_object, uname, pword, connection)
-        self.t = tapis_object
-   
+class Neo4jCLI(TapisQuery):
+    """
+    @help: integrated CLI to interface with Neo4j pods
+    """
     @decorators.RequiresExpression
-    def submit_query(self, file: str, id: str, expression: str) -> str: # function to submit queries to a Neo4j knowledge graph
+    def query(self, id: str, expression: str) -> str: # function to submit queries to a Neo4j knowledge graph
         uname, pword = self.t.pods.get_pod_credentials(pod_id=id).user_username, self.t.pods.get_pod_credentials(pod_id=id).user_password
         graph = Graph(f"bolt+ssc://{id}.pods.icicle.tapis.io:443", auth=(uname, pword), secure=True, verify=True)
-        if file:
-            with open(file, 'r') as f:
-                expression = f.read()
-        
+
         try:
             return_value = graph.run(expression)
             print(type(return_value))
             if str(return_value) == '(No data)' and 'create' in expression.lower(): # if no data is returned (mostly if something is created) then just say 'success'
                 return f'[+][{id}@pods.icicle.tapis.io:443] Success'
             elif str(return_value) == '(No data)':
                 return f'[-][{id}@pods.icicle.tapis.io:443] KG is empty'
 
+            print(return_value)
+            print(type(return_value))
             return str(f'[+][{id}] {return_value}')
         except Exception as e:
             return str(e)
 
 
 class Pods(tapisObject):
     """
```

### Comparing `TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.24
+Version: 0.0.25
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
-1. `pip install TapisCL-ICICLE`. Ensure your version is 0.0.24
+1. `pip install TapisCL-ICICLE`. Current version 0.0.24
 2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
 **Full Terminal Interface:**
```

### Comparing `TapisCL-ICICLE-0.0.24/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.25/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.24/pyproject.toml` & `TapisCL-ICICLE-0.0.25/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.24"
+version = "0.0.25"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

