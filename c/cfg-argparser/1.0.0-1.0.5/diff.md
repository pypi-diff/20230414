# Comparing `tmp/cfg-argparser-1.0.0.tar.gz` & `tmp/cfg-argparser-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-argparser-1.0.0.tar", last modified: Wed Apr 12 21:07:07 2023, max compression
+gzip compressed data, was "cfg-argparser-1.0.5.tar", last modified: Fri Apr 14 04:14:49 2023, max compression
```

## Comparing `cfg-argparser-1.0.0.tar` & `cfg-argparser-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-12 21:07:07.896548 cfg-argparser-1.0.0/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.0.0/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      450 2023-04-12 21:07:07.896548 cfg-argparser-1.0.0/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       65 2023-04-12 20:56:15.000000 cfg-argparser-1.0.0/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      612 2023-04-12 21:06:49.000000 cfg-argparser-1.0.0/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-04-12 21:07:07.896548 cfg-argparser-1.0.0/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-12 21:07:07.896548 cfg-argparser-1.0.0/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-12 21:07:07.896548 cfg-argparser-1.0.0/src/cfg_argparser/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      103 2023-04-12 20:53:57.000000 cfg-argparser-1.0.0/src/cfg_argparser/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    11745 2023-04-12 20:49:51.000000 cfg-argparser-1.0.0/src/cfg_argparser/config_arg_parser.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-12 21:07:07.896548 cfg-argparser-1.0.0/src/cfg_argparser.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      450 2023-04-12 21:07:07.000000 cfg-argparser-1.0.0/src/cfg_argparser.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      265 2023-04-12 21:07:07.000000 cfg-argparser-1.0.0/src/cfg_argparser.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-04-12 21:07:07.000000 cfg-argparser-1.0.0/src/cfg_argparser.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-04-12 21:07:07.000000 cfg-argparser-1.0.0/src/cfg_argparser.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.0.5/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1493 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      962 2023-04-14 03:38:02.000000 cfg-argparser-1.0.5/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      597 2023-04-14 04:14:31.000000 cfg-argparser-1.0.5/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/src/cfg_argparser/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      104 2023-04-12 21:18:54.000000 cfg-argparser-1.0.5/src/cfg_argparser/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    11355 2023-04-14 04:09:51.000000 cfg-argparser-1.0.5/src/cfg_argparser/config_arg_parser.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1493 2023-04-14 04:14:49.000000 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      265 2023-04-14 04:14:49.000000 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-04-14 04:14:49.000000 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-04-14 04:14:49.000000 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/top_level.txt
```

### Comparing `cfg-argparser-1.0.0/LICENSE` & `cfg-argparser-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.0.0/src/cfg_argparser/config_arg_parser.py` & `cfg-argparser-1.0.5/src/cfg_argparser/config_arg_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         self.load()
         return self
 
     def save(self, out_dict=None, indent=4):
         if not isinstance(out_dict, dict):
             out_dict = self
         with open(self.cfg_path, 'w+') as f:
-            print(out_dict)
             f.write(json.dumps(out_dict, indent=indent))
         return self
 
     def update(self, *args, **kwargs):
         super().update(*args, **kwargs)
         return self
 
@@ -201,73 +200,63 @@
                 original[key] = {}
             update_from_flattened(original[key], {future: value})
         else:
             original[key] = value
 
 
 class ConfigArgParser:
-    '''Creates an easy argparse config utility.
-    It saves given args to a path, and returns them when args are parsed again.'''
+    '''an easy argparse config utility. It saves given args to a json, and returns them when args are parsed again.'''
 
-    def __init__(self, parser: ArgumentParser,
-                 config_path, cfgObject: CfgDict = None, exit_on_change: bool = False):
-        '''An argparse config utility made to wrap an ArgumentParser
-
-        Parameters:
-        parser: argparse.ArgumentParser -- argparse function.
-        config_path: str -- a path to the supposed json file
-        exit_on_change: bool -- when commands set and reset are passed, exit once finished.
-
-        '''
+    def __init__(self,
+                 parser: ArgumentParser,
+                 config_path: str,
+                 cfgObject: CfgDict = None,
+                 exit_on_change: bool = False,
+                 argument_group_name: str = "Config options"):
+        """Constructs a parser wrapper.
+
+        Parameters
+        ----------
+        parser : ArgumentParser
+            parser to wrap.
+        config_path : str
+            the path to the json file.
+        cfgObject : CfgDict, optional
+            if desired, update an existing CfgDict object, by default None
+        exit_on_change : bool, optional
+            exits when set, reset, or reset_all is called, by default False
+        argument_group_name : str, optional
+            name of the argument group, by default "Config options"
+        
+        """
 
         # parent parser
-        self._parent = parser
-        self.config_path = config_path
-        self.default_prefix = self._parent.prefix_chars[0]
+        self.parser = parser
+        self.default_prefix = self.parser.prefix_chars[0]
         self.exit_on_change = exit_on_change
         self.file = cfgObject or CfgDict(config_path)
 
-        # set up subparser
-        self.parser = ArgumentParser(
-            prog=self._parent.prog,
-            usage=self._parent.usage,
-            description=self._parent.description,
-            epilog=self._parent.epilog,
-            parents=[self._parent],
-            formatter_class=self._parent.formatter_class,
-            prefix_chars=self._parent.prefix_chars,
-            fromfile_prefix_chars=self._parent.fromfile_prefix_chars,
-            argument_default=self._parent.argument_default,
-            conflict_handler=self._parent.conflict_handler,
-            add_help=False,
-            allow_abbrev=self._parent.allow_abbrev,
-            exit_on_error=True
-        )
-
         # Add config options
-        self.config_option_group = self.parser.add_argument_group(
-            'Config options')
+        self.config_option_group = self.parser.add_argument_group(argument_group_name)
         self.config_options = self.config_option_group.add_mutually_exclusive_group()
         self.config_options.add_argument(self.default_prefix * 2 + "set", nargs=2, metavar=('KEY', 'VAL'),
                                          help="change a default argument's options")
         self.config_options.add_argument(self.default_prefix * 2 + "reset", metavar='VALUE', nargs="*",
                                          help="removes a changed option.")
         self.config_options.add_argument(self.default_prefix * 2 + "reset_all", action="store_true",
                                          help="resets every option.")
 
         # get defaults from the actions
         # self.parser_tree = get_parser_tree(self._parent)
-        self.parser_tree = ParserTree(self._parent)
-
-        self.file.load()
+        self.parser_tree = ParserTree(self.parser)
 
     def parse_args(self, **kwargs) -> Namespace:
-        '''args.set, reset, reset_all logic'''
+        '''args.set, reset, reset_all logic. Also a passthrough for parser.parse_args.'''
 
-        # print(required_args)
+        self.file.load()
 
         # Add subparsers to the dict so it can be configured
         self.parser_tree.update_from_flattened(ParserTree.flatten(self.file))
 
         self.kwargs = ParserTree.flatten(self.parser_tree.get_defaults())
 
         # disable every required item that wasn in the file
@@ -305,15 +294,16 @@
         ParserTree.reenable_required(still_required)
 
         # sys_exit()
         self.parser.parse_args()
 
         return self.parser_tree.parse()
 
-    def _convert_type(self, potential_args: list) -> list:
+    @staticmethod
+    def _convert_type(potential_args: list) -> list:
         arg_replacements = {"true": True, "false": False,
                             "none": None, "null": None}
         potential_args[1] = arg_replacements.get(
             potential_args[1].lower(), potential_args[1])
         if str(potential_args[1]).isdigit():
             potential_args[1] = int(potential_args[1])
         return potential_args
```

