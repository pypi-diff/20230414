# Comparing `tmp/ansible-variables-0.3.1.tar.gz` & `tmp/ansible-variables-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-variables-0.3.1.tar", last modified: Thu Apr 13 21:13:21 2023, max compression
+gzip compressed data, was "ansible-variables-0.4.0.tar", last modified: Fri Apr 14 14:16:13 2023, max compression
```

## Comparing `ansible-variables-0.3.1.tar` & `ansible-variables-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.511618 ansible-variables-0.3.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.511618 ansible-variables-0.3.1/lib/ansible_variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/lib/ansible_variables/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/lib/ansible_variables/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/lib/ansible_variables/utils/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/lib/ansible_variables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 21:13:21.000000 ansible-variables-0.3.1/lib/ansible_variables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:13:21.515618 ansible-variables-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-13 21:13:09.000000 ansible-variables-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.220984 ansible-variables-0.4.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/lib/ansible_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/lib/ansible_variables/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/lib/ansible_variables/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/lib/ansible_variables/utils/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/lib/ansible_variables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 14:16:13.000000 ansible-variables-0.4.0/lib/ansible_variables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:13.224984 ansible-variables-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-14 14:16:00.000000 ansible-variables-0.4.0/tests/test_variablesource.py
```

### Comparing `ansible-variables-0.3.1/LICENSE` & `ansible-variables-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.3.1/lib/ansible_variables/cli/variables.py` & `ansible-variables-0.4.0/lib/ansible_variables/cli/variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 
 from ansible import context
 from ansible.cli import CLI
 from ansible.cli.arguments import option_helpers as opt_help
 from ansible.errors import AnsibleOptionsError
 from ansible.utils.display import Display
 
-from ansible_variables.utils.vars import variable_sources, source_mapping
+from ansible_variables.utils.vars import variable_sources
 
 display = Display()
 
 # Internal vars same as defined for ansible-inventory
-# (https://github.com/ansible/ansible/blob/d081ed36169f4f74512d1707909185281a30e29b/lib/ansible/cli/inventory.py#L28-L46)
+# pylint: disable=line-too-long
+# (https://github.com/ansible/ansible/blob/d081ed36169f4f74512d1707909185281a30e29b/lib/ansible/cli/inventory.py#L28-L46
 INTERNAL_VARS = frozenset(
     [
         "ansible_diff_mode",
         "ansible_config_file",
         "ansible_facts",
         "ansible_forks",
         "ansible_inventory_sources",
@@ -41,21 +42,21 @@
 
 class VariablesCLI(CLI):
     """used to display from where a variable value is comming from"""
 
     name = "ansible-variables"
 
     def __init__(self, args):
-        super(VariablesCLI, self).__init__(args)
+        super().__init__(args)
         self.loader = None
         self.inventory = None
-        self.vm = None
+        self.vm = None  # pylint: disable=invalid-name
 
-    def init_parser(self):
-        super(VariablesCLI, self).init_parser(
+    def init_parser(self, usage="", desc=None, epilog=None):
+        super().init_parser(
             usage="usage: %prog [options] [host]",
             epilog="Show variable sources for a host.",
         )
 
         opt_help.add_inventory_options(self.parser)
         opt_help.add_vault_options(self.parser)
         opt_help.add_basedir_options(self.parser)
@@ -80,39 +81,45 @@
             action="store",
             default=None,
             dest="variable",
             help="Only check for specific variable",
         )
 
     def post_process_args(self, options):
-        options = super(VariablesCLI, self).post_process_args(options)
+        options = super().post_process_args(options)
 
         display.verbosity = options.verbosity
         self.validate_conflicts(options)
 
         return options
 
     def run(self):
-        super(VariablesCLI, self).run()
+        super().run()
 
         # Initialize needed objects
         self.loader, self.inventory, self.vm = self._play_prereqs()
+        verbosity = context.CLIARGS["verbosity"]
 
         host = self.inventory.get_host(context.CLIARGS["host"])
         if not host:
             raise AnsibleOptionsError("You must pass a single valid host to ansible-variables")
 
-        for var, value, source in variable_sources(
-            vm=self.vm,
+        for variable in variable_sources(
+            variable_manager=self.vm,
             host=host,
             var=context.CLIARGS["variable"],
-            verbosity=context.CLIARGS["verbosity"],
         ):
-            if var not in INTERNAL_VARS:
-                rich.print(f"[bold]{var}[/bold]: {value} - [italic]{source_mapping(source)}[/italic]")
+            if variable.name not in INTERNAL_VARS:
+                rich.print(
+                    f"[bold]{variable.name}[/bold]: {variable.value} - [italic]{variable.source_mapped}[/italic]"
+                )
+                if verbosity >= 1:
+                    files = variable.file_occurrences(loader=self.loader)
+                    for ffile in files:
+                        rich.print(ffile)
 
 
 def main(args=None):
     VariablesCLI.cli_executor(args)
 
 
 if __name__ == "__main__":
```

### Comparing `ansible-variables-0.3.1/lib/ansible_variables.egg-info/SOURCES.txt` & `ansible-variables-0.4.0/lib/ansible_variables.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 lib/ansible_variables.egg-info/requires.txt
 lib/ansible_variables.egg-info/top_level.txt
 lib/ansible_variables/cli/__init__.py
 lib/ansible_variables/cli/variables.py
 lib/ansible_variables/utils/__init__.py
 lib/ansible_variables/utils/vars.py
 tests/test_cli.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_variablesource.py
```

### Comparing `ansible-variables-0.3.1/setup.cfg` & `ansible-variables-0.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [metadata]
 name = ansible-variables
-version = 0.3.1
-description = Check from where Ansible inventory variables are comming from
+version = 0.4.0
+description = Keep track of Ansible host context variables
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Christoph Hille
 author_email = hille721@gmail.com
 url = https://github.com/hille721/ansible-variables
 project_urls = 
 	Bug Tracker=https://github.com/hille721/ansible-variables/issues
-	Documentation=https://github.com/hille721/ansible-variables
+	Documentation=https://github.com/hille721/ansible-variables/blob/main/README.md
 license = GPLv3+
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Natural Language :: English
 	Operating System :: POSIX
@@ -49,11 +49,17 @@
 [options.entry_points]
 console_scripts = 
 	ansible-variables = ansible_variables.cli.variables:main
 
 [flake8]
 max-line-length = 120
 
+[pylint.format]
+max-line-length = 120
+
+[pylint."message control"]
+disable = missing-module-docstring, missing-function-docstring, consider-using-f-string
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ansible-variables-0.3.1/tests/test_cli.py` & `ansible-variables-0.4.0/tests/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     assert "ansible-variables: error: the following arguments are required: host" in capsys.readouterr().err
 
 
 def test_cli_config(capsys):
     variables_cli = VariablesCLI(["ansible-variables", "--version"])
     with pytest.raises(SystemExit):
         variables_cli.run()
-    assert C.CONFIG_FILE in capsys.readouterr().out.splitlines()[1]
+    assert "tests/test_data/ansible.cfg" in capsys.readouterr().out.splitlines()[1]
 
 
 def test_cli_from_all(capsys):
     for server in ["server1", "server2", "server3"]:
         variables_cli = VariablesCLI(["ansible-variables", server, "--var", "from_all"])
         variables_cli.run()
         captured = capsys.readouterr()
-        assert "from_all: hello - group_vars (all)" == captured.out.strip()
+        assert "from_all: hello - inventory group_vars/all" == captured.out.strip()
```

