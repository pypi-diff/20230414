# Comparing `tmp/testflows.connect-1.7.210811.1000931.tar.gz` & `tmp/testflows.connect-1.7.230414.1210340.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.connect-1.7.210811.1000931.tar", last modified: Wed Aug 11 00:09:31 2021, max compression
+gzip compressed data, was "testflows.connect-1.7.230414.1210340.tar", last modified: Fri Apr 14 21:03:40 2023, max compression
```

## Comparing `testflows.connect-1.7.210811.1000931.tar` & `testflows.connect-1.7.230414.1210340.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-08-11 00:09:31.525587 testflows.connect-1.7.210811.1000931/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2020-09-12 20:32:34.000000 testflows.connect-1.7.210811.1000931/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       16 2020-09-12 20:32:34.000000 testflows.connect-1.7.210811.1000931/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     1425 2021-08-11 00:09:31.525587 testflows.connect-1.7.210811.1000931/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      568 2020-09-12 20:32:34.000000 testflows.connect-1.7.210811.1000931/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2021-08-11 00:09:31.525587 testflows.connect-1.7.210811.1000931/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1611 2021-08-11 00:09:31.000000 testflows.connect-1.7.210811.1000931/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-08-11 00:09:31.525587 testflows.connect-1.7.210811.1000931/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-08-11 00:09:31.525587 testflows.connect-1.7.210811.1000931/testflows/connect/
--rw-rw-r--   0 user      (1000) user      (1000)     1416 2021-08-11 00:09:31.000000 testflows.connect-1.7.210811.1000931/testflows/connect/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    13294 2021-08-11 00:08:46.000000 testflows.connect-1.7.210811.1000931/testflows/connect/shell.py
--rw-rw-r--   0 user      (1000) user      (1000)     2337 2021-05-07 19:46:33.000000 testflows.connect-1.7.210811.1000931/testflows/connect/ssh.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-08-11 00:09:31.525587 testflows.connect-1.7.210811.1000931/testflows.connect.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1425 2021-08-11 00:09:31.000000 testflows.connect-1.7.210811.1000931/testflows.connect.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      364 2021-08-11 00:09:31.000000 testflows.connect-1.7.210811.1000931/testflows.connect.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2021-08-11 00:09:31.000000 testflows.connect-1.7.210811.1000931/testflows.connect.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2020-09-19 15:51:15.000000 testflows.connect-1.7.210811.1000931/testflows.connect.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       27 2021-08-11 00:09:31.000000 testflows.connect-1.7.210811.1000931/testflows.connect.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2021-08-11 00:09:31.000000 testflows.connect-1.7.210811.1000931/testflows.connect.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:03:40.721303 testflows.connect-1.7.230414.1210340/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-03-13 19:58:24.000000 testflows.connect-1.7.230414.1210340/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       16 2023-03-13 19:58:24.000000 testflows.connect-1.7.230414.1210340/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-04-14 21:03:40.721303 testflows.connect-1.7.230414.1210340/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      448 2023-03-13 19:58:26.000000 testflows.connect-1.7.230414.1210340/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-14 21:03:40.721303 testflows.connect-1.7.230414.1210340/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1577 2023-04-14 21:03:40.000000 testflows.connect-1.7.230414.1210340/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:03:40.721303 testflows.connect-1.7.230414.1210340/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:03:40.721303 testflows.connect-1.7.230414.1210340/testflows/connect/
+-rw-rw-r--   0 user      (1000) user      (1000)     1416 2023-04-14 21:03:40.000000 testflows.connect-1.7.230414.1210340/testflows/connect/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13644 2023-04-14 21:00:32.000000 testflows.connect-1.7.230414.1210340/testflows/connect/shell.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2540 2023-04-14 21:00:32.000000 testflows.connect-1.7.230414.1210340/testflows/connect/ssh.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:03:40.721303 testflows.connect-1.7.230414.1210340/testflows.connect.egg-info/
+-rwxrwxr-x   0 user      (1000) user      (1000)     1008 2023-04-14 21:03:40.000000 testflows.connect-1.7.230414.1210340/testflows.connect.egg-info/PKG-INFO
+-rwxrwxr-x   0 user      (1000) user      (1000)      379 2023-04-14 21:03:40.000000 testflows.connect-1.7.230414.1210340/testflows.connect.egg-info/SOURCES.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)        1 2023-04-14 21:03:40.000000 testflows.connect-1.7.230414.1210340/testflows.connect.egg-info/dependency_links.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)        1 2022-12-23 06:55:08.000000 testflows.connect-1.7.230414.1210340/testflows.connect.egg-info/not-zip-safe
+-rwxrwxr-x   0 user      (1000) user      (1000)       27 2023-04-14 21:03:40.000000 testflows.connect-1.7.230414.1210340/testflows.connect.egg-info/requires.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)       10 2023-04-14 21:03:40.000000 testflows.connect-1.7.230414.1210340/testflows.connect.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:03:40.721303 testflows.connect-1.7.230414.1210340/tests/
+-rwxrwxr-x   0 user      (1000) user      (1000)     8656 2023-04-14 21:03:20.000000 testflows.connect-1.7.230414.1210340/tests/tests.py
```

### Comparing `testflows.connect-1.7.210811.1000931/LICENSE` & `testflows.connect-1.7.230414.1210340/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.connect-1.7.210811.1000931/PKG-INFO` & `testflows.connect-1.7.230414.1210340/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 Metadata-Version: 2.1
 Name: testflows.connect
-Version: 1.7.210811.1000931
+Version: 1.7.230414.1210340
 Summary: TestFlows - Connect
 Home-page: https://github.com/testflows/testflows-connect
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
-Description: # TestFlows - Connect
-        
-        **The connect module is still work in progress and is currently under development.
-        Please use it only for reference.**
-        
-        Minimal module to provide capabilities to connect to
-        and control CLI programs.
-        
-        Currently supports only Python 3.6 or above.
-        
-        ## Installation
-        
-        ```bash
-            $ ./build; ./install
-        ```
-        
-        where
-        
-        ```bash
-            $ ./build
-        ```
-        
-        creates a pip installable package in `./dist`, for example
-        
-        ```bash
-            $ ls dist/
-            testflows.connect-1.2.190905.123636.tar.gz
-        ```
-        
-        and
-        
-        ```bash
-            $ ./install
-        ```
-        
-        installs the `testflows.connect` module.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# TestFlows - Connect
+
+Minimal module to provide capabilities to connect to
+and control CLI programs.
+
+Currently supports only Python 3.6 or above.
+
+## Installation
+
+```bash
+    $ ./build; ./install
+```
+
+where
+
+```bash
+    $ ./build
+```
+
+creates a pip installable package in `./dist`, for example
+
+```bash
+    $ ls dist/
+    testflows.connect-1.2.190905.123636.tar.gz
+```
+
+and
+
+```bash
+    $ ./install
+```
+
+installs the `testflows.connect` module.
```

### Comparing `testflows.connect-1.7.210811.1000931/setup.py` & `testflows.connect-1.7.230414.1210340/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,35 +15,31 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name="testflows.connect",
-    version="1.7.210811.1000931",
+    version="1.7.230414.1210340",
     description="TestFlows - Connect",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/testflows/testflows-connect",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
     license="Apache-2.0",
     packages=[
         "testflows.connect",
     ],
     zip_safe=False,
     install_requires=[
-        #"testflows.uexpect"
+        # "testflows.uexpect"
     ],
-    extras_require={
-        "dev": [
-            "testflows.core>=1.6"
-        ]
-    }
+    extras_require={"dev": ["testflows.core>=1.6"]},
 )
```

### Comparing `testflows.connect-1.7.210811.1000931/testflows/connect/__init__.py` & `testflows.connect-1.7.230414.1210340/testflows/connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.7.210811.1000931"
+__version__ = "1.7.230414.1210340"
 __license__ = f"""
 Copyright 2019 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.connect-1.7.210811.1000931/testflows/connect/shell.py` & `testflows.connect-1.7.230414.1210340/testflows/connect/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 from collections import namedtuple
 
 from testflows.core import current
 from testflows.uexpect import spawn, ExpectTimeoutError
 
 __all__ = ["Shell", "Parser"]
 
+
 class Application(object):
     """Base class for all CLI applications
     launched and controlled using uExpect.
     """
+
     pass
 
 
 class Parser(object):
     def __init__(self, pattern, types=None):
         if types is None:
             types = {}
@@ -74,40 +76,42 @@
         self.execute()
 
     def get_exitcode(self):
         if getattr(self.app.commands, "get_exitcode", None) is None:
             return None
 
         while True:
-            if not self.app.child.expect(self.app.prompt, timeout=0.001, expect_timeout=True):
+            if not self.app.child.expect(
+                self.app.prompt, timeout=0.001, expect_timeout=True
+            ):
                 break
- 
+
         command = self.app.commands.get_exitcode
-        
+
         self.app.child.send(command, eol="")
         self.app.child.expect(re.escape(command))
         self.app.child.send("\r", eol="")
         self.app.child.expect("\n")
         self.app.child.expect(self.app.prompt)
-        
+
         return int(self.app.child.before.rstrip().replace("\r", ""))
 
     def execute(self):
         self.app._send_command(self.command)
 
         next_timeout = self.timeout
         if next_timeout is None:
             next_timeout = sys.maxsize
 
         start_time = time.time()
         pattern = f"({self.app.prompt})|(\n)"
 
         while True:
             raised_timeout = False
-            
+
             try:
                 match = self.app.child.expect(pattern, timeout=next_timeout)
 
                 if not self.output:
                     self.output = ""
 
                 if match.groups()[0]:
@@ -121,20 +125,22 @@
 
                     if self.total:
                         if elapsed >= self.total:
                             raised_timeout = True
                             raise ExpectTimeoutError(match.re, self.total, self.output)
                         next_timeout = max(self.timeout, self.total - elapsed)
                         continue
-            
+
             except ExpectTimeoutError:
                 if not raised_timeout:
-                    self.output = self.app.child.before \
-                        if self.output is None \
-                        else (self.output + (self.app.child.before or ''))
+                    self.output = (
+                        self.app.child.before
+                        if self.output is None
+                        else (self.output + (self.app.child.before or ""))
+                    )
                 elapsed = time.time() - start_time
 
                 if self.total:
                     if elapsed >= self.total:
                         raise
                     next_timeout = max(self.timeout, self.total - elapsed)
                     continue
@@ -148,25 +154,33 @@
 
         self.exitcode = self.get_exitcode()
         self.app.child.send("\r", eol="")
         self.app.child.expect("\n")
 
         return self
 
+
 class AsyncCommand(Command):
-    """Asynchronous command.
-    """
+    """Asynchronous command."""
+
     def __init__(self, app, command, timeout=None, parser=None, name=None):
         if timeout is None:
             timeout = 0.5
 
         if name is None:
             name = command
 
-        super(AsyncCommand, self).__init__(app=app, command=command, timeout=timeout, total=None, parser=parser, name=name)
+        super(AsyncCommand, self).__init__(
+            app=app,
+            command=command,
+            timeout=timeout,
+            total=None,
+            parser=parser,
+            name=name,
+        )
 
     def execute(self):
         self.app._send_command(self.command)
 
     def __enter__(self):
         return self
 
@@ -185,16 +199,15 @@
         if self.exitcode is None:
             self.app.child.send(ctrl, eol="")
             output += self.readlines()
 
         return output
 
     def readlines(self, timeout=None, test=None):
-        """Return currently available output.
-        """
+        """Return currently available output."""
         if test is None:
             test = current()
 
         if timeout is None:
             timeout = self.timeout
 
         if self.app.test is not test:
@@ -217,52 +230,56 @@
                     self.app.child.expect("\n")
                     break
                 # new line
                 elif match.groups()[1]:
                     output += self.app.child.before + self.app.child.after
 
             except ExpectTimeoutError:
-                output = self.app.child.before \
-                    if output is None \
-                    else (output + (self.app.child.before or ''))
+                output = (
+                    self.app.child.before
+                    if output is None
+                    else (output + (self.app.child.before or ""))
+                )
                 break
 
         output = output.rstrip().replace("\r", "")
 
         if output and self.parser:
             self.values = self.parser.parse(output)
 
         if self.output is None:
             self.output = ""
 
         self.output += output
         return output
 
+
 ShellCommands = namedtuple("ShellCommands", "change_prompt get_exitcode")
 
+
 class Shell(Application):
     """Connection to shell application.
 
     :param command: command to launch shell, default: ["/bin/bash", "--noediting"]
     :param prompt: prompt, default: r'[#\$] '
     :param change_prompt: command to change promptm default: None
     :param new_prompt: new prompt to set, default: None
     """
+
     name = "bash"
-    prompt = r'[#\$] '
+    prompt = r"[#\$] "
     new_prompt = "bash# "
-    command = ["/bin/bash", "--noediting"]
-    commands = ShellCommands(
-        change_prompt="export PS1=\"{}\"",
-        get_exitcode="echo $?"
-        )
+    command = ["/bin/bash", "--noediting", "--norc", "--noprofile"]
+    commands = ShellCommands(change_prompt='export PS1="{}"', get_exitcode="echo $?")
     timeout = 10
     multiline_prompt = ">"
 
-    def __init__(self, command=None, prompt=None, new_prompt=None, name=None, spawn=spawn):
+    def __init__(
+        self, command=None, prompt=None, new_prompt=None, name=None, spawn=spawn
+    ):
         self.command = command or self.command
         self.prompt = prompt or self.prompt
         self.new_prompt = new_prompt or self.new_prompt
         self.child = None
         self.test = None
         self.spawn = spawn
         self.name = name if name is not None else self.name
@@ -282,21 +299,21 @@
 
         if self.test is not test:
             self.test = test
             self.child.logger(self.test.message_io(self.name))
 
         if self.new_prompt and getattr(self.commands, "change_prompt", None):
             self.child.expect(self.prompt)
-            
+
             change_prompt_command = self.commands.change_prompt.format(self.new_prompt)
-            
+
             self.child.send(change_prompt_command)
             self.child.expect(re.escape(change_prompt_command))
             self.child.expect("\n")
-            
+
             self.prompt = self.new_prompt
 
     def close(self):
         if self.child:
             child = self.child
             self.child = None
             child.close()
@@ -332,42 +349,52 @@
         if self.test is not test:
             self.test = test
             self.child.logger(self.test.message_io(self.name))
 
         return self.child.expect(*args, **kwargs)
 
     def _send_command(self, command, timeout=60):
-        """Send command.
-        """
+        """Send command."""
         self.child.expect(self.prompt)
 
         while True:
             if not self.child.expect(self.prompt, timeout=0.001, expect_timeout=True):
                 break
 
         lines = command.strip().split("\n")
 
         for i, line in enumerate(lines):
             if i > 0:
                 self.child.send("\n", eol="")
                 self.child.expect("\n")
-                self.child.expect(self.multiline_prompt, timeout=self.timeout, expect_timeout=False)
+                self.child.expect(
+                    self.multiline_prompt, timeout=self.timeout, expect_timeout=False
+                )
 
             if line:
                 self.child.send(line, eol="")
 
         while True:
             if not self.child.expect("\n", timeout=0.001, expect_timeout=True):
                 break
 
         self.child.send("\r", eol="")
         self.child.expect("\n", timeout=timeout)
 
-    def __call__(self, command, timeout=None, total=None, parser=None, asynchronous=False,
-            asyncronous=False, test=None, name=None):
+    def __call__(
+        self,
+        command,
+        timeout=None,
+        total=None,
+        parser=None,
+        asynchronous=False,
+        asyncronous=False,
+        test=None,
+        name=None,
+    ):
         """Execute shell command.
 
         :param command: command to execute
         :param timeout: time to wait for the next line of output
         :param total: time to wait for the command to complete
             and return to the prompt, default: None (no limit)
         :param parser: output parser
@@ -383,25 +410,34 @@
         if self.child is None:
             self.open(timeout)
 
         if self.test is not test:
             self.test = test
 
         if asyncronous or asynchronous:
-            return AsyncCommand(self, command=command, timeout=None, parser=parser, name=name)
-
-        return Command(self, command=command, timeout=timeout, total=total, parser=parser, name=name)
+            return AsyncCommand(
+                self, command=command, timeout=None, parser=parser, name=name
+            )
+
+        return Command(
+            self,
+            command=command,
+            timeout=timeout,
+            total=total,
+            parser=parser,
+            name=name,
+        )
 
     def __exit__(self, type, value, traceback):
         self.close()
 
     @contextmanager
     def subshell(self, command, name="sub-bash", prompt=None):
-        """Open subshell in the current shell.
-        """
+        """Open subshell in the current shell."""
+
         def spawn(command):
             self.expect(self.prompt)
             self.send(command)
             return self.child
 
         def close():
             pass
@@ -412,21 +448,22 @@
         child_close = self.child.close
         child_timeout = self.child.timeout
         child_eol = self.child.eol
 
         try:
             self.child.close = close
 
-            with Shell(spawn=spawn, command=command, name=name, prompt=prompt) as sub_shell:
+            with Shell(
+                spawn=spawn, command=command, name=name, prompt=prompt
+            ) as sub_shell:
                 try:
                     yield sub_shell
                 finally:
                     sub_shell.send("exit")
                     sub_shell.expect("exit")
                     sub_shell.expect(self.prompt)
                     sub_shell.send("")
                     sub_shell.expect("\n")
         finally:
             self.child.close = child_close
             self.child.timeout = child_timeout
             self.child.eol = child_eol
-
```

### Comparing `testflows.connect-1.7.210811.1000931/testflows/connect/ssh.py` & `testflows.connect-1.7.230414.1210340/testflows/connect/ssh.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,32 +14,48 @@
 # limitations under the License.
 from contextlib import contextmanager
 
 from .shell import Shell
 
 __all__ = ["SSH"]
 
+
 @contextmanager
-def SSH(host, username, password=None, command="{client} {username}@{host} {options}",
-        client="ssh", options=["-v"], port=None, prompt=r"[\$#] ", new_prompt="bash# "):
-    """Open SSH terminal to a remote host.
-    """
+def SSH(
+    host,
+    username,
+    password=None,
+    command="{client} {username}@{host} {options}",
+    client="ssh",
+    options=["-v"],
+    port=None,
+    prompt=r"[\$#] ",
+    new_prompt="bash# ",
+):
+    """Open SSH terminal to a remote host."""
     if options is None:
         options = []
 
     if port is not None:
         options.append(f"-p {port}")
 
     with Shell(name=f"ssh-{host}") as bash:
-        command = command.format(client=client, username=username, host=host, options=" ".join(options).strip())
+        command = command.format(
+            client=client,
+            username=username,
+            host=host,
+            options=" ".join(options).strip(),
+        )
 
         bash.send(command)
 
-        c = bash.expect(r"(Last login)|(Could not resolve hostname)|(Connection refused)|"
-            r"(Are you sure you want to continue connecting)")
+        c = bash.expect(
+            r"(Last login)|(Could not resolve hostname)|(Connection refused)|"
+            r"(Are you sure you want to continue connecting)"
+        )
 
         if c.group() == "Are you sure you want to continue connecting":
             bash.send("yes", delay=0.5)
             c = bash.expect(r"(Last login)")
 
         if c.group() == "Last login":
             bash.expect(prompt)
@@ -58,13 +74,19 @@
         child_close = bash.child.close
         child_timeout = bash.child.timeout
         child_eol = bash.child.eol
 
         try:
             bash.child.close = close
 
-            with Shell(spawn=spawn, name=host, prompt=prompt, command=[""], new_prompt=new_prompt) as ssh:
+            with Shell(
+                spawn=spawn,
+                name=host,
+                prompt=prompt,
+                command=[""],
+                new_prompt=new_prompt,
+            ) as ssh:
                 yield ssh
         finally:
             bash.child.close = child_close
             bash.child.timeout = child_timeout
             bash.child.eol = child_eol
```

### Comparing `testflows.connect-1.7.210811.1000931/testflows.connect.egg-info/PKG-INFO` & `testflows.connect-1.7.230414.1210340/testflows.connect.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 Metadata-Version: 2.1
 Name: testflows.connect
-Version: 1.7.210811.1000931
+Version: 1.7.230414.1210340
 Summary: TestFlows - Connect
 Home-page: https://github.com/testflows/testflows-connect
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
-Description: # TestFlows - Connect
-        
-        **The connect module is still work in progress and is currently under development.
-        Please use it only for reference.**
-        
-        Minimal module to provide capabilities to connect to
-        and control CLI programs.
-        
-        Currently supports only Python 3.6 or above.
-        
-        ## Installation
-        
-        ```bash
-            $ ./build; ./install
-        ```
-        
-        where
-        
-        ```bash
-            $ ./build
-        ```
-        
-        creates a pip installable package in `./dist`, for example
-        
-        ```bash
-            $ ls dist/
-            testflows.connect-1.2.190905.123636.tar.gz
-        ```
-        
-        and
-        
-        ```bash
-            $ ./install
-        ```
-        
-        installs the `testflows.connect` module.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# TestFlows - Connect
+
+Minimal module to provide capabilities to connect to
+and control CLI programs.
+
+Currently supports only Python 3.6 or above.
+
+## Installation
+
+```bash
+    $ ./build; ./install
+```
+
+where
+
+```bash
+    $ ./build
+```
+
+creates a pip installable package in `./dist`, for example
+
+```bash
+    $ ls dist/
+    testflows.connect-1.2.190905.123636.tar.gz
+```
+
+and
+
+```bash
+    $ ./install
+```
+
+installs the `testflows.connect` module.
```

