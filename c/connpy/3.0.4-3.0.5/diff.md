# Comparing `tmp/connpy-3.0.4.tar.gz` & `tmp/connpy-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.0.4.tar", last modified: Fri Apr 14 16:47:02 2023, max compression
+gzip compressed data, was "connpy-3.0.5.tar", last modified: Fri Apr 14 21:32:13 2023, max compression
```

## Comparing `connpy-3.0.4.tar` & `connpy-3.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:02.919291 connpy-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 16:46:53.000000 connpy-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 16:47:02.919291 connpy-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-14 16:46:53.000000 connpy-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:02.919291 connpy-3.0.4/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47147 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27912 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:02.919291 connpy-3.0.4/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-14 16:47:02.919291 connpy-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 16:46:53.000000 connpy-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:32:13.171288 connpy-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 21:31:58.000000 connpy-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 21:32:13.171288 connpy-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-14 21:31:58.000000 connpy-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:32:13.171288 connpy-3.0.5/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47220 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27894 2023-04-14 21:31:58.000000 connpy-3.0.5/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:32:13.171288 connpy-3.0.5/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 21:32:13.000000 connpy-3.0.5/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-14 21:32:13.171288 connpy-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 21:31:58.000000 connpy-3.0.5/setup.py
```

### Comparing `connpy-3.0.4/LICENSE` & `connpy-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.0.4/PKG-INFO` & `connpy-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.0.4
+Version: 3.0.5
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.0.4/README.md` & `connpy-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.0.4/connpy/__init__.py` & `connpy-3.0.5/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.4/connpy/api.py` & `connpy-3.0.5/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.4/connpy/completion.py` & `connpy-3.0.5/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.4/connpy/configfile.py` & `connpy-3.0.5/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.4/connpy/connapp.py` & `connpy-3.0.5/connpy/connapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -764,15 +764,15 @@
         else:
             node["port"] = defaults["port"]
         if edit["options"]:
             questions.append(inquirer.Text("options", message="Pass extra options to protocol", validate=self._default_validation, default=defaults["options"]))
         else:
             node["options"] = defaults["options"]
         if edit["logs"]:
-            questions.append(inquirer.Text("logs", message="Pick logging path/file ", validate=self._default_validation, default=defaults["logs"]))
+            questions.append(inquirer.Text("logs", message="Pick logging path/file ",  validate=self._default_validation, default=defaults["logs"].replace("{","{{").replace("}","}}")))
         else:
             node["logs"] = defaults["logs"]
         if edit["user"]:
             questions.append(inquirer.Text("user", message="Pick username", validate=self._default_validation, default=defaults["user"]))
         else:
             node["user"] = defaults["user"]
         if edit["password"]:
@@ -824,15 +824,15 @@
         else:
             profile["port"] = defaults["port"]
         if edit["options"]:
             questions.append(inquirer.Text("options", message="Pass extra options to protocol", default=defaults["options"]))
         else:
             profile["options"] = defaults["options"]
         if edit["logs"]:
-            questions.append(inquirer.Text("logs", message="Pick logging path/file ", default=defaults["logs"]))
+            questions.append(inquirer.Text("logs", message="Pick logging path/file ", default=defaults["logs"].replace("{","{{").replace("}","}}")))
         else:
             profile["logs"] = defaults["logs"]
         if edit["user"]:
             questions.append(inquirer.Text("user", message="Pick username", default=defaults["user"]))
         else:
             profile["user"] = defaults["user"]
         if edit["password"]:
```

### Comparing `connpy-3.0.4/connpy/core.py` & `connpy-3.0.5/connpy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,28 +389,28 @@
                 cmd = cmd + " " + self.options
             if self.logs != '':
                 self.logfile = self._logfile()
             if self.password[0] != '':
                 passwords = self._passtx(self.password)
             else:
                 passwords = []
-            expects = ['yes/no', 'refused', 'supported', 'cipher', 'ssh-keygen.*\"', 'timeout', 'unavailable', 'closed', '[p|P]assword:|[u|U]sername:', r'>$|#$|\$$|>.$|#.$|\$.$', 'suspend', pexpect.EOF, pexpect.TIMEOUT, "No route to host", "resolve hostname", "no matching host key"]
+            expects = ['yes/no', 'refused', 'supported', 'cipher', 'ssh-keygen.*\"', 'timeout', 'unavailable', 'closed', '[p|P]assword:|[u|U]sername:', r'>$|#$|\$$|>.$|#.$|\$.$', 'suspend', pexpect.EOF, pexpect.TIMEOUT, "No route to host", "resolve hostname", "no matching"]
         elif self.protocol == "telnet":
             cmd = "telnet " + self.host
             if self.port != '':
                 cmd = cmd + " " + self.port
             if self.options != '':
                 cmd = cmd + " " + self.options
             if self.logs != '':
                 self.logfile = self._logfile()
             if self.password[0] != '':
                 passwords = self._passtx(self.password)
             else:
                 passwords = []
-            expects = ['[u|U]sername:', 'refused', 'supported', 'cipher', 'ssh-keygen.*\"', 'timeout', 'unavailable', 'closed', '[p|P]assword:', r'>$|#$|\$$|>.$|#.$|\$.$', 'suspend', pexpect.EOF, pexpect.TIMEOUT, "No route to host", "resolve hostname", "no matching host key"]
+            expects = ['[u|U]sername:', 'refused', 'supported', 'cipher', 'ssh-keygen.*\"', 'timeout', 'unavailable', 'closed', '[p|P]assword:', r'>$|#$|\$$|>.$|#.$|\$.$', 'suspend', pexpect.EOF, pexpect.TIMEOUT, "No route to host", "resolve hostname", "no matching"]
         else:
             raise ValueError("Invalid protocol: " + self.protocol)
         attempts = 1
         while attempts <= max_attempts:
             child = pexpect.spawn(cmd)
             if debug:
                 print(cmd)
```

### Comparing `connpy-3.0.4/connpy.egg-info/PKG-INFO` & `connpy-3.0.5/connpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.0.4
+Version: 3.0.5
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.0.4/setup.cfg` & `connpy-3.0.5/setup.cfg`

 * *Files identical despite different names*

